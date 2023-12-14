<template>
  <div class="text-center">
    <v-hover v-slot:default="{ hover }" open-delay="50">
      <v-card :elevation="hover ? 8 : 0" class="" width="220">
        <v-img
          class="pointer-cursor"
          max-width="220"
          :src="productImage"
        ></v-img>

        <v-card-text class="text-start">
          <div class="font-weight-meduim black--text">{{ productName }}</div>
          <div class="font-weight-meduim green--text">
            {{ productPrice }}
          </div>

          <div class="d-flex justify-space-between mt-2">
            <v-chip small label class="ma-0 white--text" color="blue">
              ໃໝ່
            </v-chip>
            <v-spacer></v-spacer>
            <v-chip small label outlined class="ma-0 white--text" color="blue">
              ພ້ອມສົ່ງ
            </v-chip>
          </div>
        </v-card-text>
      </v-card>
    </v-hover>
  </div>
</template>

<script>
import ProductImage from '~/assets/img/products/product_3.jpg'
export default {
  name: 'new-products-card',
  data() {
    return {
      productName: 'Hair Dryer ໄດເປົ່າຜົມ 1800W Sonifer',
      productPrice: '250,000 LAK',
      productImage: ProductImage,
    }
  },
}
</script>

<style></style>
