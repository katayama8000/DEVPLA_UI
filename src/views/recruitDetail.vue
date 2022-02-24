<template>
  <v-container>
    <v-row>
      <v-col>
        <v-avatar color="primary" size="89" />
        <div>{{title}}</div>
      </v-col>
    </v-row>
    <hr />
    <v-row>
      <v-col cols="2">
        <v-card>{{LanguageUsed[0].language}}</v-card>
      </v-col>
      <v-col cols="2">
        <v-card>{{LanguageUsed[1].language}}</v-card>
      </v-col>
      <v-col cols="2">
        <v-card>{{LanguageUsed[2].language}}</v-card>
      </v-col>
    </v-row>
    <v-btn block color="primary" shaped elevation="2" large class="ma-5">
      メッセージを送る
    </v-btn>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      title:"募集タイトル",
      LanguageUsed:[
        {language:"javaScript"},
        {language:"Ruby"},
        {language:"Laravel"}
      ],
    };
  },
};
</script>

<style>
</style>