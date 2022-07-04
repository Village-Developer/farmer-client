<template>
    <div>
        <v-row>
            <Navbar />
        </v-row>
        <v-row>
            <v-col cols="4" class="ml-16 mt-10">
                <Menu />
            </v-col>
            <v-col cols="auto" class="mt-10">
                <Display />
            </v-col>
        </v-row>
    </div>
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
