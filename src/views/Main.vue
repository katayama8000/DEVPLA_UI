<template>
  <v-container>
    <h2>募集一覧ページ</h2>
    <div align="center">
      <v-row justify="center">
        <v-col cols="6">
          <v-text-field label="検索" single-line outlined></v-text-field>
        </v-col>
      </v-row>
      <h4 class="ma-5">カテゴリ人気順</h4>
      <v-row justify="center">
        <v-col md="2">
          <div>★用途別</div>
          <div v-for="(category, index) in categories" :key="index">
            <v-card class="pa-2 ma-2" outlined tile>{{ category }}</v-card>
          </div>
        </v-col>
        <v-col md="2">
          <div>★フレームワーク</div>
          <div v-for="(category, index) in categories" :key="index">
            <v-card class="pa-2 ma-2" outlined tile>{{ category }}</v-card>
          </div>
        </v-col>
        <v-col md="2">
          <div>★プログラミング言語</div>
          <div v-for="(category, index) in categories" :key="index">
            <v-card class="pa-2 ma-2" outlined tile>{{ category }}</v-card>
          </div>
        </v-col>
        <v-col md="2">
          <div>★クラウド</div>
          <div v-for="(category, index) in categories" :key="index">
            <v-card class="pa-2 ma-2" outlined tile>{{ category }}</v-card>
          </div>
        </v-col>
        <v-col md="2">
          <div>★AI関連</div>
          <v-btn class="pa-2 px-13 ma-2" outlined tile>あああ</v-btn>
          <v-card class="pa-2 ma-2" outlined tile>あああ</v-card>
          <v-card class="pa-2 ma-2" outlined tile>あああ</v-card>
          <v-card class="pa-2 ma-2" outlined tile>あああ</v-card>
        </v-col>
      </v-row>
      <h4 class="ma-10">最近更新されたグループ</h4>
      <v-row>
        <v-col cols="3" v-for="n in 5" :key="n">
          <PostedCard />
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script>
import PostedCard from "../components/PostedCard.vue";
export default {
  components: {
    PostedCard,
  },
  data: () => ({
    categories: ["PHP", "JavaScript ", "python", "Ruby", "C言語"],
  }),
};
</script>

<style>
</style>