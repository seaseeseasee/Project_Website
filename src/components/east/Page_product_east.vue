<script setup>
import Header_box_east from '../east/Box_menu_east.vue'
import { Otop_eastStore } from '../../stores/All_product'
import { ref, computed } from 'vue'
import { addToCart } from '../shop/Cart_count.js'
import { cart } from '../shop/Cart_count'

const totalItems = computed(() => cart.value.reduce((acc, item) => acc + item.quantity, 0))

const otop_eastStore = Otop_eastStore()
const otop_east_all = ref(otop_eastStore.Otop_east_list)

const handleAddToCart = (item) => {
  addToCart(item)
}
</script>

<template>
  <!-- แถบ ภาพ  -->

  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-image-container">
        <img
          src="https://scontent.fbkk29-7.fna.fbcdn.net/v/t1.15752-9/387593657_6765877803479798_8168857763006525534_n.png?_nc_cat=106&ccb=1-7&_nc_sid=8cd0a2&_nc_eui2=AeG_Q_0LYJor6HDQQzuY5q-dYRn0stqJGyNhGfSy2okbI02Jv8YoT_GkkZohC7OS1fsGh79GWXun6dNsUVaMLMRb&_nc_ohc=XvSYrxWVwxUAX93UXfK&_nc_ht=scontent.fbkk29-7.fna&oh=03_AdRQw7yvifWje5c2OFC7PxtTytZ_vmmw2NLodz4noKCT8Q&oe=654E0959"
          class="d-block w-100"
          alt="..."
          height="450"
        />
        <router-link :to="{ name: 'main' }">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="32"
            height="32"
            fill="currentColor"
            class="bi bi-house house-icon"
            viewBox="0 0 16 16"
          >
            <path
              d="M8.707 1.5a1 1 0 0 0-1.414 0L.646 8.146a.5.5 0 0 0 .708.708L2 8.207V13.5A1.5 1.5 0 0 0 3.5 15h9a1.5 1.5 0 0 0 1.5-1.5V8.207l.646.647a.5.5 0 0 0 .708-.708L13 5.793V2.5a.5.5 0 0 0-.5-.5h-1a.5.5 0 0 0-.5.5v1.293L8.707 1.5ZM13 7.207V13.5a.5.5 0 0 1-.5.5h-9a.5.5 0 0 1-.5-.5V7.207l5-5 5 5Z"
            />
          </svg>
        </router-link>

        <!-- ตระกร้า -->
        <ul class="nav justify-content-end">
          <li class="nav-item">
            <router-link :to="{ name: 'cart' }">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="30"
                height="60"
                fill="currentColor"
                class="bi bi-cart"
                viewBox="0 0 16 16"
              >
                <path
                  d="M0 1.5A.5.5 0 0 1 .5 1H2a.5.5 0 0 1 .485.379L2.89 3H14.5a.5.5 0 0 1 .491.592l-1.5 8A.5.5 0 0 1 13 12H4a.5.5 0 0 1-.491-.408L2.01 3.607 1.61 2H.5a.5.5 0 0 1-.5-.5zM3.102 4l1.313 7h8.17l1.313-7H3.102zM5 12a2 2 0 1 0 0 4 2 2 0 0 0 0-4zm7 0a2 2 0 1 0 0 4 2 2 0 0 0 0-4zm-7 1a1 1 0 1 1 0 2 1 1 0 0 1 0-2zm7 0a1 1 0 1 1 0 2 1 1 0 0 1 0-2z"
                />
              </svg>
              <span>[ {{ totalItems }} ]</span>
            </router-link>
          </li>
          <!-- เมนู -->
          <li class="nav-item">
            <router-link :to="{ name: 'orderList' }">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="30"
                height="60"
                fill="currentColor"
                class="bi bi-card-checklist"
                viewBox="0 0 16 16"
              >
                <path
                  d="M14.5 3a.5.5 0 0 1 .5.5v9a.5.5 0 0 1-.5.5h-13a.5.5 0 0 1-.5-.5v-9a.5.5 0 0 1 .5-.5h13zm-13-1A1.5 1.5 0 0 0 0 3.5v9A1.5 1.5 0 0 0 1.5 14h13a1.5 1.5 0 0 0 1.5-1.5v-9A1.5 1.5 0 0 0 14.5 2h-13z"
                />
                <path
                  d="M7 5.5a.5.5 0 0 1 .5-.5h5a.5.5 0 0 1 0 1h-5a.5.5 0 0 1-.5-.5zm-1.496-.854a.5.5 0 0 1 0 .708l-1.5 1.5a.5.5 0 0 1-.708 0l-.5-.5a.5.5 0 1 1 .708-.708l.146.147 1.146-1.147a.5.5 0 0 1 .708 0zM7 9.5a.5.5 0 0 1 .5-.5h5a.5.5 0 0 1 0 1h-5a.5.5 0 0 1-.5-.5zm-1.496-.854a.5.5 0 0 1 0 .708l-1.5 1.5a.5.5 0 0 1-.708 0l-.5-.5a.5.5 0 0 1 .708-.708l.146.147 1.146-1.147a.5.5 0 0 1 .708 0z"
                />
              </svg>
            </router-link>
          </li>
        </ul>
      </div>
    </div>
  </div>

  <!-- แถบ menu -->
  <Header_box_east></Header_box_east>

  <!--กิจกรรมที่น่าสนใจ-->
  <div class="container">
    <h1 class="textcenter"><strong>สินค้าOTOPที่น่าสนใจ</strong></h1>
    <hr />

    <div class="row row-cols-1 row-cols-md-2 g-4">
      <div class="col" v-for="(i, index) in otop_east_all" :key="index">
        <div
          class="d-flex flex-column flex-lg-row gap-3 align-items-start align-items-lg-center py-3 link-body-emphasis text-decoration-none border-top"
        >
          <img :src="i.img" class="rounded float-start" alt="..." width="300" height="300" />
          <div class="card-body">
            <h5 class="card-text mb-auto">
              <strong class="h3">{{ i.name }}</strong>
            </h5>
            <p class="card-text">
              <strong>ประเภท: {{ i.category }}</strong>
            </p>
            <p class="card-text">
              <strong>ราคา:{{ i.price }} บาท</strong>
            </p>
            <p class="card-text">{{ i.text }}</p>
            <button
              type="submit"
              @click="handleAddToCart(i)"
              class="btn btn-dark"
              style="border-radius: 30px"
            >
              ลงตะกร้า
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
.textcenter {
  text-align: center;
  margin-inline: 420px;
  border-bottom: 2px solid;
}
</style>
