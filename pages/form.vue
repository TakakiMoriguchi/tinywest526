<template>
  <main class="form">
    <v-container
      class="jumboTron-form d-flex align-end mb-10"
      fluid
    >
      <v-container class="about-title">
        <h1>お問合せ</h1>
        <p>Contact</p>
      </v-container>
    </v-container>

    <v-container>
      <v-alert
        v-model="dialogs.isSuccess"
        dismissible
        color="green"
        border="left"
        elevation="2"
        colored-border
        icon="mdi-checkbox-marked-circle"
      >
        {{ dialogs.successMessage }}
      </v-alert>
      <v-alert
        v-model="dialogs.isFailed"
        dismissible
        color="orange"
        border="left"
        elevation="2"
        colored-border
        icon="mdi-alert"
      >
        {{ dialogs.errorMessage }}
      </v-alert>
    </v-container>

    <section class="row d-flex justify-center priceTable mb-5">
      <v-form ref="form">
        <v-text-field
          v-model="formData.name"
          label="name"
          hint="名前"
          prepend-icon="mdi-draw"
          required
        />

        <v-text-field
          v-model="formData.telephone"
          label="telephone"
          hint="電話番号"
          :rules="isNumber"
          prepend-icon="mdi-phone"
        />

        <v-text-field
          v-model="formData.email"
          label="email"
          hint="メールアドレス"
          :rules="isMailAdress"
          prepend-icon="mdi-email"
          name="_replyto"
        />

        <v-select
          v-model="formData.problem"
          :items="problems"
          label="problems"
          prepend-icon="mdi-alert"
        />

        <v-textarea
          v-model="formData.message"
          label="text"
          hint="備考"
          prepend-icon="mdi-format-color-text"
        />

        <div class="action-area">
          <v-btn
            @click="submit"
          >
            送信
          </v-btn>
        </div>
      </v-form>
    </section>

    <!-- footer -->
    <global-footer />
  </main>
</template>

<script>
import axios from 'axios'

export default {
  data () {
    return {
      dialogs: {
        isSuccess: false,
        isFailed: false,
        successMessage: '送信完了',
        errorMessage: 'default error message'
      },
      formData: {
        name: '',
        telephone: '',
        email: '',
        problem: '',
        message: ''
      },
      problems: [
        '画面修理',
        'バッテリー交換',
        'その他'
      ],
      isNumber: [
        value => !!value || 'Required.',
        (value) => {
          const pattern = /^[0-9]+$/
          return pattern.test(value) || 'Invalid Number.'
        }
      ],
      isMailAdress: [
        value => !!value || 'Required.',
        (value) => {
          const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
          return pattern.test(value) || 'Invalid e-mail.'
        }
      ]
    }
  },

  methods: {
    submit (event) {
      event.preventDefault()
      axios({
        method: 'POST',
        url: 'https://formspree.io/f/xvollpbe',
        data: this.formData
      }).then(() => {
        this.formClear()
        this.dialogs.isSuccess = true
      }).catch((error) => {
        this.formClear()
        this.dialogs.errorMessage = error.response.data.error
        this.dialogs.isFailed = true
      })
    },
    formClear () {
      this.formData.name = ''
      this.formData.telephone = ''
      this.formData.email = ''
      this.formData.problem = ''
      this.formData.message = ''
    }
  }
}
</script>
