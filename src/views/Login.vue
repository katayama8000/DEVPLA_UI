<template>
  <v-card width="400px" class="mx-auto mt-5">
    <v-card-title>
      <h1>ログイン</h1>
    </v-card-title>
    <v-card-text>
      <v-form>
        <v-text-field
          prepend-icon="mdi-account-circle"
          label="email"
          v-model="email"
        />
        <v-text-field
          v-bind:type="showPassword ? 'text' : 'password'"
          @click:append="showPassword = !showPassword"
          prepend-icon="mdi-lock"
          v-bind:append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
          label="パスワード"
          v-model="password"
        />
        <v-row class="justify-center">
          <v-btn class="ma-5" @click="submit">ログイン</v-btn>
          <v-btn class="ma-5"><router-link to="/signup">新規登録</router-link></v-btn>
        </v-row>
          <!-- <span>登録していない方はこちら → </span> -->
      </v-form>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
      showPassword: false,
      password: "",
      email: "",
    };
  },
  methods: {
    submit() {
    },
  },
};
</script>