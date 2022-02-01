<template>
  <v-app>
    <v-app-bar app>
      <router-link to="about" class="pa-5">about</router-link>
      <router-link to="home" class="pa-5">home</router-link>
      <router-link to="login" class="pa-5">login</router-link>
      <router-link to="signUp" class="pa-5">SignUp</router-link>
      <router-link to="main" class="pa-5">Main</router-link>
      <router-link to="recruitDetail" class="pa-5">recruitDetail</router-link>
    </v-app-bar>

    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    //
  }),
};
</script>
