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
          <div class="font-weight-meduim red--text">
            <span class="text-decoration-line-through"
              >{{ productPrice }}
            </span>

            <span class="black--text ml-2">({{ discountPercent }})</span>
          </div>
          <div class="font-weight-meduim green--text">
            {{ discountPrice }}
          </div>

          <div class="d-flex justify-space-between mt-2">
            <v-chip small label class="ma-0 white--text" color="green">
              ຫຼຸດລາຄາ
            </v-chip>
            <v-spacer></v-spacer>
            <v-chip small label outlined class="ma-0 white--text" color="green">
              ພ້ອມສົ່ງ
            </v-chip>
          </div>
        </v-card-text>
      </v-card>
    </v-hover>
  </div>
</template>

<script>
import ProductImage from '~/assets/img/products/product_1.jpg'
export default {
  name: 'discount-products-card',
  data() {
    return {
      productName: 'Balance Smart Watch ໂມງ Amazfit Black',
      productPrice: '219000 LAK',
      discountPrice: '119000 LAK',
      discountPercent: '-50%',
      productImage: ProductImage,
    }
  },
}
</script>

<style></style>
