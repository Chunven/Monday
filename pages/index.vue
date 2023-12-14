<template>
  <div class="mr-16 ml-16">
    <div class="brands mb-4 mt-2">
      <brands></brands>
    </div>

    <div class="discount-products mb-4">
      <v-card class="pa-6 rounded-lg">
        <v-row>
          <v-list class="" style="margin-bottom: -10px">
            <v-list-item>
              <v-avatar tile color="green rounded-pill" size="40" class="mr-2">
                <v-icon color="white">mdi-cash-minus</v-icon></v-avatar
              >
              <v-list-item-title> <h3>ສິນຄ້າຫຼຸດລາຄາ</h3> </v-list-item-title>
              <v-list-item-icon> </v-list-item-icon>
            </v-list-item>
          </v-list>
          <v-spacer />
          <v-btn text color="green" class="green--text mt-3">
            ເບິ່ງເພີ່ມເຕີມ
            <v-icon right dark> mdi-arrow-right-circle </v-icon>
          </v-btn>

          <v-col cols="12">
            <v-divider class="mb-2"></v-divider>
            <div class="row">
              <div
                v-for="(item, index) in 6"
                :key="index"
                class="col-12 col-md-2 col-sm-6 col-xs-6 text-center"
              >
                <discount-products-card></discount-products-card>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div>

    <div class="banner-1 mb-4">
      <v-card class="rounded-lg">
        <v-img max-width="100%" :src="Banner_1"></v-img>
      </v-card>
    </div>

    <div class="hot-products mb-4">
      <v-card class="pa-6 rounded-lg">
        <v-row>
          <v-list class="" style="margin-bottom: -10px">
            <v-list-item>
              <v-avatar tile color="red rounded-pill" size="40" class="mr-2">
                <v-icon color="white">mdi-fire</v-icon></v-avatar
              >
              <v-list-item-title> <h3>ສີນຄ້າຍອດນິຍົມ</h3> </v-list-item-title>
              <v-list-item-icon> </v-list-item-icon>
            </v-list-item>
          </v-list>
          <v-spacer />
          <v-btn text color="red" class="red--text mt-3">
            ເບິ່ງເພີ່ມເຕີມ
            <v-icon right dark> mdi-arrow-right-circle </v-icon>
          </v-btn>

          <v-col cols="12">
            <v-divider class="mb-2"></v-divider>
            <div class="row">
              <div
                v-for="(item, index) in 6"
                :key="index"
                class="col-12 col-md-2 col-sm-6 col-xs-6 text-center"
              >
                <hot-products-card></hot-products-card>
              </div>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div>

    <div class="banner-2 mb-4">
      <v-card class="rounded-lg">
        <v-img max-width="100%" :src="Banner_2"></v-img>
      </v-card>
    </div>

    <div class="new-products mb-4">
      <v-card class="pa-6 rounded-lg">
        <v-row>
          <v-list class="" style="margin-bottom: -10px">
            <v-list-item>
              <v-avatar tile color="blue rounded-pill" size="40" class="mr-2">
                <v-icon color="white">mdi-new-box</v-icon></v-avatar
              >
              <v-list-item-title> <h3>ສິນຄ້າໃໝ່</h3> </v-list-item-title>
              <v-list-item-icon> </v-list-item-icon>
            </v-list-item>
          </v-list>
          <v-spacer />
          <!-- <v-btn text color="blue" class="blue--text">
            ເບິ່ງເພີ່ມເຕີມ
            <v-icon right dark> mdi-arrow-right-circle </v-icon>
          </v-btn> -->

          <v-col cols="12">
            <v-divider class="mb-2"></v-divider>
            <div class="row">
              <div
                v-for="(item, index) in 12"
                :key="index"
                class="col-12 col-md-2 col-sm-6 col-xs-6 text-center"
              >
                <new-products-card></new-products-card>
              </div>
              <div class="col-12 col-md-12 col-sm-6 col-xs-6 text-center">
                <v-btn class="blue white--text" outlined>
                  ເບິ່ງເພີ່ມເຕີມ <v-icon>mdi-arrow-down</v-icon></v-btn
                >
              </div>
            </div>
          </v-col>
        </v-row>
      </v-card>
    </div>

    <!-- <div class="">
      <v-col cols="12">
        <div class="row">
          <footer></footer>
        </div>
      </v-col>
    </div> -->
  </div>
</template>

<script>
import Banner_1 from '~/assets/img/banners/banner_1.png'
import Banner_2 from '~/assets/img/banners/banner_2.png'

export default {
  data() {
    return {
      Banner_1: Banner_1,
      Banner_2: Banner_2,
      icons: ['mdi-facebook', 'mdi-whatsapp'],
    }
  },
  computed: {},
}
</script>

<style></style>
