<template>
    <v-app>
        <Navbar />
        <v-main class="grey lighten-3">
            <v-container>
                <v-row>
                    <v-col cols="2">
                        <Menu />
                    </v-col>
                    <v-col>
                        <Display />
                    </v-col>
                </v-row>
            </v-container>
        </v-main>
    </v-app>
</template>

<script>

import Navbar from '../components/Navbar.vue'
import Menu from '../components/user_manage/Menu.vue'
import Display from '../components/user_manage/Display.vue'

export default {
  name: 'UserManage',
  components: {
    Navbar,
    Menu,
    Display
  }
}
</script>

<style>

</style>
