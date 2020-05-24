<template>
  <main id="app">
    <section class="products">

      <Product 
        v-for="product in products"
        :key="product.color"
        :product="product"
      />

    </section>
  </main>
</template>

<script>
import Product from './components/Product.vue'

export default {
  name: 'App',
  components: {
    Product
  },
  data () {
    products:[
      {
        title: 'Nike Air Max',
        color: 'green',
        bgtext: 'NIKE',
        src: require('./assets/green-shoe.png')
      },
      {
        title: 'Nike Flex',
        color: 'blue',
        bgtext: 'AIR',
        src: require('./assets/blue-shoe.png')
      },
      {
        title: 'Nike Roche Runs',
        color: 'pink',
        bgtext: 'MAX',
        src: require('./assets/pink-shoe.png')
      }
    ]
  }
}
</script>

<style>

</style>
