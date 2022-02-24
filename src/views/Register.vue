<template>
  <v-container class="container">
    <div>
      <h1 class="ma-10">個人情報登録</h1>
      <v-row>
        <v-col cols="4" align-content="center">ユーザー名</v-col>
        <v-col cols="2" color="red">必須</v-col>
        <v-col cols="6"
          ><v-text-field
            v-model="userName"
            :rules="nameRules"
            label="山田太郎"
            required
            single-line
            outlined
          ></v-text-field>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="4" align-content="center">メールアドレス</v-col>
        <v-col cols="2" color="red">必須</v-col>
        <v-col cols="6"
          ><v-text-field
            v-model="firstname"
            :rules="emailRules"
            label="japan@gmail.com"
            required
            single-line
            outlined
          ></v-text-field>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="6"></v-col>
        <v-col cols="6"
          ><v-text-field
            v-model="firstname"
            :rules="emailRules"
            label="japan@gmail.com"
            required
            single-line
            outlined
          ></v-text-field>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="4" align-content="center">パスワード</v-col>
        <v-col cols="2" color="red">必須</v-col>
        <v-col cols="6"
          ><v-text-field
            v-model="firstname"
            :rules="nameRules"
            label="password"
            type="password"
            required
            single-line
            outlined
          ></v-text-field>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="6"></v-col>
        <v-col cols="6"
          ><v-text-field
            v-model="firstname"
            :rules="nameRules"
            label="password"
            type="password"
            required
            single-line
            outlined
          ></v-text-field>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="4" align-content="center">性別</v-col>
        <v-col cols="2" color="red">必須</v-col>
        <v-col cols="6">
          <v-combobox 
          outlined 
          solo
          :items="gender"
          ></v-combobox>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="4" align-content="center">プログラミング経験年数</v-col>
        <v-col cols="2" color="red">必須</v-col>
        <v-col cols="6">
          <v-combobox 
          outlined 
          solo
          :items="experience"
          ></v-combobox>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="4" align-content="center">自己紹介</v-col>
        <v-col cols="2" color="red">任意</v-col>
        <v-col cols="6">
          <v-textarea
          solo
          name="input-7-4"
          label="自己紹介"
        ></v-textarea>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    nameRules: [(v) => !!v || "Name is required"],
    emailRules: [
      (v) => !!v || "E-mail is required",
      (v) => /.+@.+/.test(v) || "E-mail must be valid",
    ],
    userName: "",
    email: "",
    gender:['男性','女性'],
    experience:['1年未満','1～3年','4～10年']
  }),
};
</script>

<style scoped>
.container {
  max-width: 750px;
}
</style>
