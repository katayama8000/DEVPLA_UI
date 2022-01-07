<template>
  <v-container>
    <v-row>
      <v-col><v-avatar color="primary" size="89" /><span>title</span></v-col>
    </v-row>
    <hr />
    <v-row>
      <v-col cols="1">
        <v-card>JavaScript</v-card>
      </v-col>
      <v-col cols="1">
        <v-card>Ruby</v-card>
      </v-col>
      <v-col cols="1">
        <v-card>Laravel</v-card>
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
      desserts: [
        {
          name: "Frozen Yogurt",
          calories: 159,
        },
        {
          name: "Ice cream sandwich",
          calories: 237,
        },
        {
          name: "Eclair",
          calories: 262,
        },
        {
          name: "Cupcake",
          calories: 305,
        },
        {
          name: "Gingerbread",
          calories: 356,
        },
        {
          name: "Jelly bean",
          calories: 375,
        },
        {
          name: "Lollipop",
          calories: 392,
        },
        {
          name: "Honeycomb",
          calories: 408,
        },
        {
          name: "Donut",
          calories: 452,
        },
        {
          name: "KitKat",
          calories: 518,
        },
      ],
    };
  },
};
</script>

<style>
</style>