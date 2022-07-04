<template>
  <v-card width="256" max-width="256" min-width="256">
    <v-navigation-drawer permanent>
        <v-system-bar></v-system-bar>
        <v-list>
            <v-list-item >
                <v-list-item-avatar>
                    <v-img src="../../assets/menu/profile.jpg"></v-img>
                </v-list-item-avatar>
            </v-list-item>

            <v-list-item link dense>
                <v-list-item-content>
                    <v-list-item-title>XeonEVO</v-list-item-title>
                    <v-list-item-subtitle>parin_boorapa@hotmail.com</v-list-item-subtitle>
                </v-list-item-content>
            </v-list-item>
        </v-list>
        <v-divider></v-divider>

        <v-list nav dense>
            <v-list-item-group>
                <v-list-item v-for="(item, i) in items" :key="i">
                    <v-list-item-content>
                        <v-list-item-title v-text="item.text"></v-list-item-title>
                    </v-list-item-content>
                </v-list-item>
            </v-list-item-group>
        </v-list>
    </v-navigation-drawer>
  </v-card>
</template>

<script>
export default {
  name: 'Menu',
  data: () => ({
    items: [
      { text: 'ตั้งค่าบัญชี' },
      { text: 'ข้อมูลส่วนตัว' },
      { text: 'ติดต่อเรา' },
      { text: 'ข้อกำหนดและเงื่อนไข' },
      { text: 'ออกจากระบบ' }
    ]
  })
}
</script>

<style>

</style>
