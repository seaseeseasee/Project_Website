<template>
  <!-- แถบ ภาพ  -->
  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-image-container">
        <img
          src="https://www.unseennewchapters.com/img/phuket-02.7d11c4d8.jpg"
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
        <h5 class="display-3">รอยพระพุทธบาทในทะเล สำนักสงฆ์เกาะแก้วพิสดาร อ</h5>
        <p class="h4">พระพุทธบาทในทะเล สำนักสงฆ์เกาะแก้วพิสดาร อ .เมือง จ.ภูเก็ต</p>
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
            src="data:image/jpeg;base64,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"
            class="d-block w-100"
            alt="..."
            height="300"
          />
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="h2"><strong>รอยพระพุทธบาทในทะเล สำนักสงฆ์เกาะแก้วพิสดาร อ</strong></h5>
            <p class="h5">
              รอยพระพุทธบาทบนทะเลแห่งนี้ เป็นรอยพระพุทธบาท รอยที่ 5 ‘นัมมทานที’ ซึ่งถือเป็น 1 ใน 5
              รอยพระพุทธบาทที่ได้รับความศรัทธาเชื่อมั่นจากพุทธศาสนิกชนทั่วโลก
              ตั้งอยู่ที่สำนักสงฆ์เกาะแก้วพิสดาร โดยช่วงเวลาน้ำทะเลขึ้นสูง
              จะไม่สามารถเห็นรอยพระพุทธบาท
              แต่เมื่อน้ำทะเลลดลงจะสามารถมองเห็นรอยพระพุทธบาทได้อย่างชัดเจน
              สามารถเดินทางท่องเที่ยวได้ตลอดทั้งปี (ยกเว้นช่วงมรสุม)
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
              ราวปี พ.ศ.2528 ได้มีพระสงฆ์จากภาคกลางรูปหนึ่งที่ชาวบ้านเรียกว่า หลวงพ่อเสือ
              ได้ธุดงค์ข้ามทะเลมาพำนักอยู่บนเกาะ และต่อมาได้ร่วมกับชาวเรือ
              ชาวน้ำในละแวกนี้พัฒนาขึ้นเป็นสำนักสงฆ์ ระยะแรกๆ แทบจะไม่มีพระรูปอื่นอยู่ด้วยเลย
              ด้วยความที่เป็นเกาะที่ไม่มีผู้คนอาศัยอยู่ การคมนาคมไม่สะดวก โดยเฉพาะในหน้ามรสุม
              การเดินทางข้ามฝั่งมายังเกาะภูเก็ตที่บริเวณหาดราไวย์ แม้จะเป็นระยะทางใกล้ๆ
              แต่ก็ยังเป็นเรื่องที่กินแรงอยู่เอาการ แม้ในทุกวันนี้ คงมีแต่พระอาจารย์เสือ
              พำนักอยู่กับพระสงฆ์รูปอื่นๆเพียงไม่กี่รูปเท่านั้น ณ
              ที่บนเกาะนี้เองที่หลวงพ่อเสือได้จัดสร้างพระเครื่องที่ต่อมามีค่านิยมสูง
              เป็นที่แสวงหาของผู้คนทั่วไป คือพระเนื้อว่านหลวงปู่ทวด และพระพ่อท่านคล้าย
              วาจาสิทธิ์..... ..... เมื่อ พ.ศ.2342 เกาะแก้วพิสดารแห่งนี้ได้ต้อนรับการมาเยือนของ
              พระยาตรังคภูมาภิบาล หรือพระยาตรัง ผู้แต่ง " นิราศถลาง "
              ซึ่งได้แต่งไว้ตอนยกทัพมาทำสงครามกับพม่าคราวศึกถลาง
              ท่านได้พรรณนาโวหารตามแบบการแต่งนิราศในสมัยนั้น คือการชมนก ชมไม้ รำลึกถึงความหลัง
              ความรัก เมื่อท่านมาถึงเกาะแก้วพิสดาร และสักการะรอยพระพุทธบาทแล้ว
              ท่านได้พรรณนาไว้ตอนหนึ่งว่า " มาประมาณโมงหนึ่งถึงพระบาท ที่กลางหาดเนินทรายชายสิงขร
              พี่ยินดีปรีดาคลายอาวรณ์ ประณมกรอภิวาทบาทบงส์ จุดธูปเทียนบุปผาบูชาพร้อม
              รินน้ำหอมปรายประชำระสรง แล้วกราบกรานคลานหมอบยอบตัวลง เหมือนพบองค์โลกนาถพระศาสดา
              ที่พบต้องมองและพระลายลักษณ์ เหมือนประจักษ์จริงจังไม่กังขา มีทั้งร้อยแปดอย่างกระจ่างตา
              เป็นดินฟ้าพรหมอินทร์สิ้นทั้งปวง "
            </p>
          </div>
        </div>
        <div class="col-md-4">
          <img
            src="https://www.unseennewchapters.com/img/phuket-01.6cf6cdf6.jpg"
            class="img-fluid rounded-start"
            alt="..."
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
        v-for="(i, index) in item_advice_south_02_all"
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
import { item_advice_south_02Store } from '../south/index_south'

const item_advice_south_02 = item_advice_south_02Store()
const item_advice_south_02_all = ref(item_advice_south_02.item_advice_south_list_02)
</script>
