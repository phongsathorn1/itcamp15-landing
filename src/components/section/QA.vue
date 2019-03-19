<template>
  <section class="home-section" id="qa">
    <div class="strip-top"></div>
    <div class="strip-bottom"></div>
    <div class="container">
      <h1 class="text-center">คำถามที่พบบ่อย</h1>
      <div class="qa-wrapper">
        <ul class="qa-list">
          <li v-for="qa in qas" :key="qa.id">
            <div class="qa-question">{{qa.question}}</div>
            <div class="qa-answer">
              <span class="answer">ตอบ</span>&nbsp;
              <span v-html="qa.answer"></span>
            </div>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      qas: [
        {
          id: 0,
          question: 'ใครสมัครค่ายนี้ได้บ้าง',
          answer: 'น้องๆ ที่ <u><b>กำลัง</b></u>ศึกษาในระดับชั้น ม.4 ถึง ม.6 และน้องๆ ที่ศึกษา ปวช. ปวส. หรือเทียบเท่า (ระดับการศึกษา อ้างอิงจากปีการศึกษา 2561)'
        },
        {
          id: 1,
          question: 'จำเป็นต้องมีพื้นฐานเกี่ยวกับคอมพิวเตอร์มาก่อนไหม',
          answer: 'ไม่จำเป็น เพราะพี่ๆ จะสอนน้องตั้งแต่ความรู้พื้นฐาน และอยู่ข้างๆตลอดการเรียนคอยช่วยเหลือน้องๆในทุกเรื่อง'
        },
        {
          id: 2,
          question: 'ค่ายนี้มีค่าใช้จ่ายอะไรบ้าง',
          answer: 'ค่าสมัครค่าย 500 บาท (จ่ายเมื่อผ่านการคัดเลือก โดยประกาศรายชื่อน้องคนที่ติดค่ายวันที่ 28 เมษายน 2562)'
        },
        {
          id: 3,
          question: 'สามารถสมัครพร้อมกันมากกว่า 1 ค่ายได้ไหม',
          answer: 'ไม่ได้ค่ะ น้องๆสามารถสมัครได้ค่ายเดียวเพียงเท่านั้น'
        },
        {
          id: 4,
          question: 'รับสมัครน้องๆจำนวนเท่าไหร่',
          answer: 'จำนวน 120 คน'
        },
        {
          id: 5,
          question: 'เป็นค่ายค้างคืน หรือค่ายแบบไป-กลับ หากค้างคืนต้องพักที่ไหน',
          answer: 'เป็นค่ายแบบค้างคืน โดยค้างที่คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง'
        },
        {
          id: 6,
          question: 'สิ่งที่ต้องใช้ในการสมัคร เอกสารต่างๆที่ต้องใช้',
          answer: 'เอกสาร ปพ.1 ของทางโรงเรียน'
        },
        {
          id: 7,
          question: 'ค่ายนี้จัดที่ไหน',
          answer: 'คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
#qa {
  padding: 50px 0px;
  background: #ebebeb;
}
#qa .strip-top {
  background: #ebebeb;
  width: 100%;
  height: 50%;
  position: absolute;
  top: -45px;
  transform: skewY(3deg);
  z-index: 99;
}

#qa .strip-bottom {
  background: #ebebeb;
  width: 100%;
  height: 50%;
  position: absolute;
  bottom: -45px;
  transform: skewY(-3deg);
  z-index: 99;
}

#qa .container {
  position: relative;
  z-index: 100;
}

#qa .answer {
  font-weight: 600;
  background: #eea113;
  display: inline-block;
  padding: 3px 10px;
}

.qa-list {
  padding: 0px;
  list-style: none;
}

.qa-list li {
  padding: 0px;
  margin-bottom: 20px;
  // text-align: center;
}

.qa-list .qa-question {
  font-size: 1.1em;
  font-weight: 500;
}

#qa .qa-wrapper {
  padding: 50px 0px;
}
</style>
