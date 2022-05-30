<template>
  <div>
    <v-app-bar
      app
      color="diago"
      dark
    >
      <v-btn
        href="/"
        text
      >
        <span class="mr-2">Home</span>
      </v-btn>

      <v-btn
        href="/dashboard"
        text
      >
        <span class="mr-2">Dashboard</span>
      </v-btn>

      <v-btn
        href="/about"
        text
      >
        <span class="mr-2">About</span>
      </v-btn>

      <v-spacer></v-spacer>

      <v-btn
        href="/login"
        text
      >
        <span class="mr-2">Login</span>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>
