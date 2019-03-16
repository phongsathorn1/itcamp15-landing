<template>
  <lazy-component>
    <section class="home-section" id="register">
      <div class="strip-top"></div>
      <div class="container">
        <h1 class="text-center">เลือกสาขาที่คุณต้องการ</h1>
        <span class="subhead text-center">คลิกค่ายที่ต้องการเพื่อดูรายละเอียดและสมัคร</span>
        <div class="register-wrapper">
          <div class="register-block app-camp" @click="show('app')">
            <div class="register-icon-wrapper">
              <div class="register-icon">
                <div class="inner-register-icon">
                  <img src="@/assets/camp/app.png">
                </div>
              </div>
            </div>
            <div class="register-detail">
              <div class="register-title">Appermort</div>
              <div class="register-status" v-if="showStatus">
                สมัครแล้ว
                <b>30 คน</b>
              </div>
            </div>
          </div>
          <div class="register-block network-camp" @click="show('network')">
            <div class="register-icon-wrapper">
              <div class="register-icon">
                <div class="inner-register-icon">
                  <img src="@/assets/camp/network.png">
                </div>
              </div>
            </div>
            <div class="register-detail">
              <div class="register-title">Netherine</div>
              <div class="register-status" v-if="showStatus">
                สมัครแล้ว
                <b>30 คน</b>
              </div>
            </div>
          </div>
          <div class="register-block data-camp" @click="show('data')">
            <div class="register-icon-wrapper">
              <div class="register-icon">
                <div class="inner-register-icon">
                  <img src="@/assets/camp/data.png">
                </div>
              </div>
            </div>
            <div class="register-detail">
              <div class="register-title">Dragota</div>
              <div class="register-status" v-if="showStatus">
                >
                สมัครแล้ว
                <b>0 คน</b>
              </div>
            </div>
          </div>
          <div class="register-block game-camp" @click="show('game')">
            <div class="register-icon-wrapper">
              <div class="register-icon">
                <div class="inner-register-icon">
                  <img src="@/assets/camp/game.png">
                </div>
              </div>
            </div>
            <div class="register-detail">
              <div class="register-title">GrindelGame</div>
              <div class="register-status" v-if="showStatus">
                >
                สมัครแล้ว
                <b>0 คน</b>
              </div>
            </div>
          </div>
          <div class="register-block iot-camp" @click="show('iot')">
            <div class="register-icon-wrapper">
              <div class="register-icon">
                <div class="inner-register-icon">
                  <img src="@/assets/camp/iot.png">
                </div>
              </div>
            </div>
            <div class="register-detail">
              <div class="register-title">Dobby of Things</div>
              <div class="register-status" v-if="showStatus">
                สมัครแล้ว
                <b>0 คน</b>
              </div>
            </div>
          </div>
        </div>
        <camp-detail
          :logo="camp.logo"
          :campname="camp.name"
          :detail="camp.detail"
          :color="camp.color"
          :id="camp.id"
          v-if="showCampdetail"
        ></camp-detail>
      </div>
    </section>
  </lazy-component>
</template>

<script>
import CampDetail from '@/components/CampDetail.vue'

export default {
  components: {
    CampDetail
  },
  data () {
    return {
      camps: [
        {
          id: 'app',
          name: 'Appermort',
          logo: 'app.png',
          color: '#1fb4ec',
          detail: 'Appermort จะพาคุณมารู้จักกับจอมวายร้ายที่คุณอาจยังไม่รู้ตัว ที่เป็นต้นเหตุหลักทำให้เหล่าผู้คน ติดมือถือกันจนงมงาย เราจะสอนศาสตร์มืดเหล่านี้ให้คุณ นำไปเผยแพร่และ<b>ดึงดูดผู้คน</b>ที่เป็นเป้าหมาย<b>ให้มาติดกับดัก App ของเรา จนต้องเปย์ตัว เปย์ใจ ให้กับ App ของคุณ</b> มาสิ ตามพวกเรามาสิ แล้วคุณจะเป็นผู้สร้างโลกใบใหม่นี้ด้วยตัวคุณเอง ... ฮ่าๆๆ'
        },
        {
          id: 'network',
          name: 'Netherine',
          logo: 'network.png',
          color: '#d61732',
          detail: 'เวทมนตร์แห่งการเชื่อมต่อที่ไม่มีสิ้นสุดจะนำพาให้เราได้มารู้จักกัน ใน Netherine จะพาน้อง ๆ ไป<b>ไขปริศนาของเทคโนโลยีการเชื่อมต่อระหว่างอุปกรณ์</b> จนเกิดขึ้นเป็นเครือข่าย อะไรทำให้เหล่าอุปกรณ์วิเศษเหล่านี้สามารถแลกเปลี่ยนข้อมูลกันได้ แต่ละอุปกรณ์รู้จักกันได้อย่างไร ที่นี่มีคำตอบ!!'
        },
        {
          id: 'game',
          name: 'GrindelGame',
          logo: 'game.png',
          color: '#6c980d',
          detail: '<b>"หากว่าเป็นผู้เล่นจนพอใจแล้ว ลองมาเป็นผู้สร้างดูไหม ?"</b> น้องๆ จะได้เรียนรู้จากศาสตร์นี้ เกี่ยวกับการสร้างเกม รู้ว่าเกมหนึ่งเกมควรจะมีอะไรบ้าง และ วิธีที่จะถ่ายทอดจินตนาการของน้อง ๆ สู่เกมที่เราสามารถเล่นได้จริง ด้วยโปรแกรม Construct 2 ที่ใช้งานได้ง่ายเข้าใจไม่ยาก เพราะความสนุกไม่ได้มีแค่ตอนเล่นเกม มาเป็นส่วนหนึ่งในค่าย GrindelGame และสร้างสรรค์เกมไปด้วยกัน!'
        },
        {
          id: 'data',
          name: 'Dragota',
          logo: 'data.png',
          color: '#9013fe',
          detail: 'พร้อมรึยังกับค่าย Dragota ศาสตร์ที่จะนำข้อมูลอันสุดแสนจะธรรมดาเปลี่ยนให้กลายเป็น<b>การพยากรณ์อนาคตที่น่าเหลือเชื่อด้วยRapidminer</b> ดั่งเวทย์มนต์ที่รังสรรค์สิ่งมหัศจรรย์ที่ไม่รู้จบ พี่ๆ พร้อมที่จะมอบความรู้ ความอบอุ่น และความสนุกให้แบบไม่อั้น แล้วน้องๆ จะรู้ว่าข้อมูลรอบตัวเรานั้นสามารถทำอะไรได้มากกว่ที่คิด!'
        },
        {
          id: 'iot',
          name: 'Dobby of Things',
          logo: 'iot.png',
          color: '#f5a623',
          detail: '“เมื่ออินเตอร์เน็ตสามารถเข้าถึงสิ่งต่างๆที่มีอยู่รอบๆตัวเราจะดีเท่าไหนกัน หากเราสามารถเสกเวทมตร์ควบคุบเครื่องใช้ไฟฟ้าให้มันเป็นดั่งใจเราได้” ศาสตร์แห่ง Dobby of Things จะพาน้องๆพบเจอกับเวทมนตร์Arduino IDE, VS Code และอื่นๆ อีกมากมายที่จะช่วยให้เราสะดวกสบายมากยิ่งขึ้น <b>ให้อินเทอร์เน็ตเปรียบเสมือน Dobby ประจําบ้านของน้องๆ</b>'
        }
      ],
      showCampdetail: false,
      selected: '',
      showStatus: false
    }
  },
  methods: {
    show (camp) {
      console.log('click')
      this.showCampdetail = true
      this.selected = camp
    }
  },
  computed: {
    camp () {
      console.log(this.camps.filter(x => x.id === this.selected)[0])
      return this.camps.filter(x => x.id === this.selected)[0]
    }
  }
}
</script>

<style lang="scss" scoped>
#register {
  padding-top: 80px;
  padding-bottom: 150px;
}

#register h1 {
  color: #333333;
}

#register .strip-top {
  background: #ffffff;
  width: 100%;
  height: 50%;
  position: absolute;
  top: -45px;
  transform: skewY(-3deg);
  z-index: 99;
}

#register .container {
  position: relative;
  z-index: 100;
  min-height: 400px;
}

#register .register-wrapper {
  display: flex;
  justify-content: space-between;
  padding-top: 30px;
  padding-bottom: 50px;
}

#register .register-block {
  margin: 0px 20px;
  width: 100%;
  cursor: pointer;
  padding-bottom: 20px;
  padding-top: 50px;
}

#register .register-block:hover {
  box-shadow: 1px 2px 10px 0px rgba(0, 0, 0, 0.4);
}

#register .register-icon-wrapper {
  position: relative;
  transform: rotate(45deg);
  height: 120px;
  width: 120px;
  margin: auto;
}

#register .app-camp .register-icon-wrapper {
  border: 2px solid #1fb4ec;
  padding: 5px;
}

#register .network-camp .register-icon-wrapper {
  border: 2px solid #d61732;
  padding: 5px;
}

#register .data-camp .register-icon-wrapper {
  border: 2px solid #9013fe;
  padding: 5px;
}

#register .game-camp .register-icon-wrapper {
  border: 2px solid #6c980d;
  padding: 5px;
}

#register .iot-camp .register-icon-wrapper {
  border: 2px solid #f5a623;
  padding: 5px;
}

#register .register-detail {
  margin-top: 50px;
  text-align: center;
}

#register .register-detail .register-title,
#register .register-detail b {
  font-weight: 600;
}

#register .app-camp .register-title {
  color: #1fb4ec;
}

#register .network-camp .register-title {
  color: #d61732;
}

#register .data-camp .register-title {
  color: #9013fe;
}

#register .game-camp .register-title {
  color: #6c980d;
}

#register .iot-camp .register-title {
  color: #f5a623;
}

#register .iot-camp .register-title {
  color: #f5a623;
}

#register .inner-register-icon {
  height: 120px;
  width: 120px;
  transform: rotate(-45deg);
  padding: 10px;
}

#register .inner-register-icon img {
  display: block;
  width: 100%;
}

@media (max-width: 768px) {
  #register .register-block {
    padding: 0px 25px;
  }
}

@media (max-width: 1024px) {
  #register .register-block {
    padding: 0px 15px;
    padding-top: 30px;
  }

  #register .register-wrapper {
    overflow-x: scroll;
  }
}
</style>
