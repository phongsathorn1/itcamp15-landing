<template>
  <section class="home-section" id="register">
    <div class="strip-top"></div>
    <div class="container">
      <h1 class="text-center">เลือกสาขาที่คุณต้องการ</h1>
      <span class="subhead text-center">คลิกค่ายที่ต้องการเพื่อดูรายละเอียดและสมัคร</span>
      <div class="register-wrapper">
        <div class="register-block app-camp">
          <div class="register-icon-wrapper">
            <div class="register-icon">
              <div class="temp-register-icon">
                <img src="../../assets/camp/app.png">
              </div>
            </div>
          </div>
          <div class="register-detail">
            <div class="register-title">Appermort</div>
            <div class="register-subtitle">พัฒนาแอปพลิเคชั่น</div>
            <div class="register-status" v-if="showStatus">
              สมัครแล้ว
              <b>0 คน</b>
            </div>
          </div>
        </div>
        <div class="register-block network-camp">
          <div class="register-icon-wrapper">
            <div class="register-icon">
              <div class="temp-register-icon"></div>
            </div>
          </div>
          <div class="register-detail">
            <div class="register-title">Netherine</div>
            <div class="register-subtitle">เน็ตเวิร์ค</div>
            <div class="register-status" v-if="showStatus">
              สมัครแล้ว
              <b>30 คน</b>
            </div>
          </div>
        </div>
        <div class="register-block data-camp">
          <div class="register-icon-wrapper">
            <div class="register-icon">s
              <div class="temp-register-icon"></div>
            </div>
          </div>
          <div class="register-detail">
            <div class="register-title">Dragota</div>
            <div class="register-subtitle">วิเคราะห์ข้อมูล</div>
            <div class="register-status" v-if="showStatus">
              >
              สมัครแล้ว
              <b>0 คน</b>
            </div>
          </div>
        </div>
        <div class="register-block game-camp">
          <div class="register-icon-wrapper">
            <div class="register-icon">
              <div class="temp-register-icon"></div>
            </div>
          </div>
          <div class="register-detail">
            <div class="register-title">GrindelGame</div>
            <div class="register-subtitle">พัฒนาเกมส์</div>
            <div class="register-status" v-if="showStatus">
              >
              สมัครแล้ว
              <b>0 คน</b>
            </div>
          </div>
        </div>
        <div class="register-block iot-camp">
          <div class="register-icon-wrapper">
            <div class="register-icon">
              <div class="temp-register-icon"></div>
            </div>
          </div>
          <div class="register-detail">
            <div class="register-title">Dobby of Things</div>
            <div class="register-subtitle">อินเตอร์เน็ตแห่งสรรพสิ่ง</div>
            <div class="register-status" v-if="showStatus">
              สมัครแล้ว
              <b>0 คน</b>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data () {
    return {
      showStatus: false
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

// #register .subhead{
//   color: #1f1f1f;
// }

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
}

#register .register-wrapper {
  display: flex;
  justify-content: space-between;
  padding-top: 100px;
  padding-bottom: 50px;
}

#register .register-block {
  margin: 0px 20px;
  width: 100%;
}

#register .register-icon-wrapper {
  position: relative;
  transform: rotate(45deg);
  height: 120px;
  width: 120px;
  margin: auto;
}

#register .app-camp .register-icon-wrapper {
  border: 2px solid #9013fe;
  padding: 5px;
}

#register .network-camp .register-icon-wrapper {
  border: 2px solid #f5a623;
  padding: 5px;
}

#register .data-camp .register-icon-wrapper {
  border: 2px solid #1fb4ec;
  padding: 5px;
}

#register .game-camp .register-icon-wrapper {
  border: 2px solid #6c980d;
  padding: 5px;
}

#register .iot-camp .register-icon-wrapper {
  border: 2px solid #d61732;
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
  color: #9013fe;
}

#register .network-camp .register-title {
  color: #f5a623;
}

#register .data-camp .register-title {
  color: #1fb4ec;
}

#register .game-camp .register-title {
  color: #6c980d;
}

#register .iot-camp .register-title {
  color: #d61732;
}

#register .temp-register-icon {
  display: flex;
  height: 120px;
  width: 120px;
  transform: rotate(-45deg);
  justify-content: center;
  align-items: center;

  img {
    width: 100%;
    height: auto;
  }
}

@media (max-width: 768px) {
  #register .register-wrapper {
    overflow-x: scroll;
  }
  #register .register-block {
    padding: 0px 25px;
  }
}
</style>
