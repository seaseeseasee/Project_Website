<template>
  <!-- แถบ ภาพ  -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-image-container">
        <img
          src="https://www.suratthanitourism.com/wp-content/uploads/2019/08/%E0%B8%AD%E0%B8%B8%E0%B8%97%E0%B8%A2%E0%B8%B2%E0%B8%99%E0%B8%98%E0%B8%A3%E0%B8%A3%E0%B8%A1%E0%B9%80%E0%B8%82%E0%B8%B2%E0%B8%99%E0%B8%B2%E0%B9%83%E0%B8%99%E0%B8%AB%E0%B8%A5%E0%B8%A7%E0%B8%87_06.jpg"
          class="d-block w-100"
          alt="..."
          height="550"
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
      </div>
      <div class="carousel-caption d-none d-md-block">
        <h5 class="display-3">อุทยานธรรมเขานาในหลวง อ.พนม จ.สุราษฎร์ธานี</h5>
        <p class="h4">อุทยานธรรมชาติที่สวยและงดงามเหมาะแก่การมาเยี่ยมชม ซักครั้ง</p>
      </div>
    </div>
  </div>

  <!-- แถบ menu -->
  <Header_box_south></Header_box_south>

  <!-- แถบ เนื้อหา -->

  <!-- box รูปซ้าย -->
  <div class="container">
    <div class="card mb-3" style="max-width: 1500px">
      <div class="row g-0">
        <div class="col-md-4">
          <img
            src="https://s.isanook.com/tr/0/ud/281/1409765/ghf.jpg"
            class="img-fluid rounded-start"
            alt="..."
          />
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="h2"><strong>อุทยานธรรมเขานาในหลวง อ.พนม จ.สุราษฎร์ธานี</strong></h5>
            <p class="h5">
              อุทยานธรรมเขานาในหลวง เป็นสำนักสงฆ์ที่สร้างขึ้นด้วยพลังศรัทธาของชาวบ้าน
              สถานที่แห่งนี้เป็นที่รู้จักจากความวิจิตรของประตูพุทธวดี หรือซุ้มประตูแห่งกาลเวลา
              ถือเป็นไฮไลต์อันแสนงดงามยามเมื่อแสงเช้าตกกระทบ ก่อนจะต่อยอดพลังศรัทธา
              ด้วยการสร้างเจดีย์ร้อยยอดพันองค์ เจดีย์ลอยฟ้าพุทธศิลาวดี เจดีย์ลอยฟ้าพุทธราชาวดี
              ทำให้ปัจจุบันสถานที่แห่งนี้เป็นเหมือนสวรรค์บนดิน โดยเฉพาะยามทะเลหมอกที่สวยงามอย่างมาก
              และเจดีย์แต่ละองค์จะดูคล้ายกับลอยอยู่บนก้อนเมฆ เป็นภาพอุทยานธรรมลอยฟ้าที่ดูตื่นตา
              และน่าอัศจรรย์ใจ นักท่องเที่ยวสามารถเดินทางมาชมความมหัศจรรย์ได้ตลอดทั้งปี
            </p>
          </div>
        </div>
      </div>
    </div>

    <!--box รูปขวา-->
    <div class="card mb-3" style="max-width: 1500px">
      <div class="row g-0">
        <div class="col-md-8">
          <div class="card-body">
            <p class="h5">
              ตามประวัติของพื้นที่บริเวณเขานาในคือ มีกลุ่มชาวบ้านราว 40 คน อพยพจาก อ.ชะอวด
              จ.นครศรีธรรมราช เข้ามาตั้งรกรากครั้งแรกในปี พ.ศ. 2518
              ซึ่งขณะนั้นพื้นที่บริเวณเขานาในอยู่ภายใต้การครอบครองของพรรคคอมมิวนิสต์แห่งประเทศไทย
              กลุ่มชาวบ้านจึงส่งตัวแทนเข้าเจรจาเพื่อขออยู่อาศัยและบุกเบิกพื้นที่ทำมาหากิน
              ต่อมาชาวบ้านจากพื้นที่อื่นๆ ทราบข่าวจึงทยอยตามเข้ามาสมทบ
              ก่อนที่พรรคคอมมิวนิสต์จะยุติบทบาทการสู้รบกับรัฐบาลไทยลงในปี พ.ศ. 2525
              ชุมชนจึงได้ขยายตัว มีการก่อตั้งวัด โรงเรียน สถานีอนามัย พัฒนาระบบสาธารณูปโภคขึ้น
              รวมถึงอุทยานธรรมที่สวยงาม สงบ และร่มรื่นแห่งนี้
            </p>
          </div>
        </div>
        <div class="col-md-4">
          <img
            src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRj1cUue3D_2rl_1uYCb1eHUdQrp5LspIrMiA&usqp=CAU"
            class="d-block w-100"
            alt="..."
            height="300"
          />
        </div>
      </div>
    </div>

    <!-- สิ่งของแนะนำขาย -->
    <h1 class="textcenter"><strong>แนะนำสินค้า</strong></h1>
    <hr />

    <div class="row row-cols-1 row-cols-md-2 g-4">
      <div
        class="card mb-3"
        style="max-width: 1500px"
        v-for="(i, index) in item_advice_south_01_all"
        :key="index"
      >
        <div class="row g-0">
          <div class="col-md-4">
            <img :src="i.img" class="img-fluid rounded-start" alt="..." />
          </div>
          <div class="col-md-8">
            <div class="card-body">
              <h5 class="card-title">{{ i.name }}</h5>
              <p class="card-text">{{ i.category }}</p>
              <button type="button" class="btn btn-dark" style="border-radius: 30px">
                LINK สินค้า
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <p class="card-text">
    <small class="text-body-secondary">
      <a class="btn btn-outline-secondary" href="https://travel.trueid.net/detail/kW22p6w5JexW"
        >อ้างอิงมาจาก</a
      ></small
    >
  </p>
</template>
<style scoped>
.textcenter {
  text-align: center;
  margin-inline: 500px;
  border-bottom: 2px solid;
}
</style>
<script setup>
import Header_box_south from '../south/Box_menu_south.vue'

import { ref } from 'vue'
import { item_advice_south_01Store } from '../south/index_south'

const item_advice_south_01 = item_advice_south_01Store()
const item_advice_south_01_all = ref(item_advice_south_01.item_advice_south_list_01)
</script>
