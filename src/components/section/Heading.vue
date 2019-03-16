<template>
  <div id="heading-container">
    <div class="container">
      <div id="heading-content">
        <img src="../../assets/logo.png" alt>
        <div class="camp">
          <h2>ไอทีแคมป์ ครั้งที่ 15</h2>
          <h1>Magic Academy</h1>
          <div class="camp-date">
            <p>31 พฤษภาคม - 2 มิถุนายน 2562</p>
            <span>คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง</span>
          </div>
        </div>
      </div>
    </div>
    <Sponsor/>
    <div class="strip-bottom"></div>
  </div>
</template>

<script>
import Sponsor from '@/components/section/Sponsor.vue'
export default {
  components: {
    Sponsor
  }
}
</script>

<style lang="scss" scoped>
#heading-container {
  background-image: url(../../assets/header.jpg);
  background-size: cover;
  background-repeat: no-repeat;
  background: #000;
  width: 100%;
  position: relative;
  padding-top: 200px;
}

#heading-content {
  text-align: center;
  margin-bottom: 100px;
}

#heading-content .camp {
  margin-top: 20px;
}

#heading-content .camp p {
  margin: 0px;
}

#heading-content .camp-date p {
  font-weight: 500;
}

#heading-container .strip-bottom {
  background-image: linear-gradient(to top, #000000, rgba(0, 0, 0, 0));
  width: 100%;
  height: 20%;
  position: absolute;
  bottom: -45px;
  transform: skewY(3deg);
  z-index: 99;
}

#heading-container .camp-date {
  margin-top: 20px;
}

span {
  font-size: 1.3em;
  color: #fff;
}

p {
  font-size: 1.5em;
  color: #fff;
}

h2 {
  color: #fff;
  font-size: 1.6em;
  font-weight: 500;
}

h1 {
  color: #f9ba47;
  font-size: 2em;
  font-weight: 600;
}
</style>
