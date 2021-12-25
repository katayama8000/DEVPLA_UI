<template>
  <v-card height="300px">
    <v-row>
      <v-col cols="8">
        <v-card-text>{{ PostedDataTitle }}</v-card-text>
      </v-col>
      <v-col cols="1">
        <v-btn class="ma-2" text icon color="blue lighten-2">
          <v-icon>mdi-thumb-up</v-icon>{{goodCount}}
        </v-btn>
      </v-col>
    </v-row>
    <v-btn class="mx-1">hello</v-btn>
    <v-btn class="mx-1">hello</v-btn>
    <v-btn class="mx-1">hello</v-btn>
    <div class="pa-5">
      xxxxxxxxxxxxxxxxxxxxxxxxxxx<br />
      xxxxxxxxxxxxxxxxxxxxxxxxxxx<br />
      xxxxxxxxxxxxxxxxxxxxxxxxxxx
    </div>
    <v-text-field
      solo
      label="メッセージを送る"
      append-icon="mdi-map-marker"
      class="px-3"
      rounded
    ></v-text-field>
  </v-card>
</template>


<script>
export default {
  data: () => ({
    PostedDataTitle: "App開発",
    goodCount:1,
  }),
};
</script>

<style>
</style>