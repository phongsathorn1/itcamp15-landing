<template>
  <div id="regsiter-wrapper">
    <h1>เลือกสาขาที่คุณต้องการ</h1>
    <h3>คลิกค่ายที่ต้องการเพื่อดูรายละเอียดและสมัคร</h3>
    <div id="register-container">
      <div class="register-card">
        <div class="register-card-wrapper" id="register-app-border">
          <div class="register-card-box"></div>
        </div>
        <h2 id="register-app">Appermort</h2>
        <p>พัฒนาแอปพลิเคชั่น</p>
        <h3>สมัครแล้ว 0 คน</h3>
      </div>
      <div class="register-card">
        <div class="register-card-wrapper" id="register-network-border">
          <div class="register-card-box"></div>
        </div>
        <h2 id="register-network">Netherine</h2>
        <p>พัฒนาแอปพลิเคชั่น</p>
        <h3>สมัครแล้ว 0 คน</h3>
      </div>
      <div class="register-card">
        <div class="register-card-wrapper" id="register-data-border">
          <div class="register-card-box"></div>
        </div>
        <h2 id="register-data">Dragota</h2>
        <p>พัฒนาแอปพลิเคชั่น</p>
        <h3>สมัครแล้ว 0 คน</h3>
      </div>
      <div class="register-card">
        <div class="register-card-wrapper" id="register-game-border">
          <div class="register-card-box"></div>
        </div>
        <h2 id="register-game">GrindelGame</h2>
        <p>พัฒนาแอปพลิเคชั่น</p>
        <h3>สมัครแล้ว 0 คน</h3>
      </div>
      <div class="register-card">
        <div class="register-card-wrapper" id="register-iot-border">
          <div class="register-card-box"></div>
        </div>
        <h2 id="register-iot">Dobby of Things</h2>
        <p>พัฒนาแอปพลิเคชั่น</p>
        <h3>สมัครแล้ว 0 คน</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
#regsiter-wrapper {
  width: 100%;
  text-align: center;
  padding-top: 5em;

  h1 {
    font-weight: 500;
    font-size: 2em;
  }

  h3 {
    font-weight: 200;
  }
}

#register-container {
  display: flex;
  justify-content: center;
  margin-top: 5em;
  margin-bottom: 10em;
}

.register-card-wrapper {
  margin: 0 2em;
  padding: 1em;
  width: 200px;
  text-align: center;
}

.register-card-box {
  width: 100%;
  height: 200px;
  background-color: #888;
}

.register-card {
  h2 {
    text-align: center;
    margin-top: 0.7em;
  }

  h3 {
    font-weight: 400;
  }

  p {
    margin-top: -0.5em;
  }
}

#register-app {
  color: #9013fe;
}

#register-app-border {
  border: #9013fe 1px solid;
}

#register-network {
  color: #f5a623;
}

#register-network-border {
  border: #f5a623 1px solid;
}

#register-data {
  color: #1fb4ec;
}

#register-data-border {
  border: #1fb4ec 1px solid;
}

#register-game {
  color: #6c980d;
}

#register-game-border {
  border: #6c980d 1px solid;
}

#register-iot {
  color: #d61732;
}

#register-iot-border {
  border: #d61732 1px solid;
}
</style>
