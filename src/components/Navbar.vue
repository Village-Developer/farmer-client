<template>
  <v-app-bar app color="deep-purple" dark>
    <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
    <v-container class="py-0 fill-height">
      <v-toolbar-title class="mr-10">Farmer Project</v-toolbar-title>
      <v-btn text>text</v-btn>
      <v-btn text>text</v-btn>
      <v-btn text>text</v-btn>
      <v-btn text>text</v-btn>
      <v-spacer></v-spacer>
      <v-avatar size="32" color="grey">
        <img src="../assets/menu/profile.jpg" alt="alt" link>
      </v-avatar>
    </v-container>
  </v-app-bar>

  <!-- <v-navigation-drawer v-model="drawer" absolute temporary>
      <v-list nav dense>
        <v-list-item-group v-model="group" active-class="deep-purple--text text--accent-4">
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Account</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer> -->
</template>

<script>
export default {
  name: 'Nabar',
  data: () => ({
    drawer: false,
    group: null,
    links: [
      'Home',
      'Dashboard',
      'User Management'
    ]
  })
}
</script>

<style>
</style>
