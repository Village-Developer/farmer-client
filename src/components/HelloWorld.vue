<template>
  <div>
    <h1>This is home page.</h1>
    <v-data-table
    dense
    :headers="headers"
    :items="info"
    item-key="name"
    class="elevation-1"
  ></v-data-table>
  </div>
</template>

<script>

export default {
  name: 'Table',

  data: () => ({
    info: [],
    headers: [
      { text: 'Product Name', value: 'productName' },
      { text: 'Detail', value: 'detail' },
      { text: 'Price', value: 'price' }
    ],
    cards: [
      { title: 'Pre-fab homes', src: 'https://cdn.vuetifyjs.com/images/cards/house.jpg', flex: 12 },
      { title: 'Favorite road trips', src: 'https://cdn.vuetifyjs.com/images/cards/road.jpg', flex: 6 },
      { title: 'Best airlines', src: 'https://cdn.vuetifyjs.com/images/cards/plane.jpg', flex: 6 }
    ]
  }),
  mounted () {
    this.axios
      .get('https://farmer-server.herokuapp.com/products')
      .then(response => (this.info = response.data))
  }
}
</script>
