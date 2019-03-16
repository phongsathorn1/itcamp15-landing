<template>
  <div id="heading-container">
    <div id="heading-content">
      <img src="../../assets/logo.png" alt>
      <h2>ไอทีแคมป์ ครั้งที่ 15</h2>
      <h1>มนตราราตรี ไอทีผู้พิทักษ์</h1>
      <p>31 พฤษภาคม - 2 มิถุนายน 2562</p>
      <span>คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง</span>
    </div>
    <Sponsor/>
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
  width: 100%;
  height: calc(100vh - 200px);
  padding-top: 200px;
}

#heading-content {
  text-align: center;
}

span {
  font-size: 1.3em;
  font-weight: 200;
  color: #fff;
}

p {
  margin-top: -0.6em;
  font-size: 1.5em;
  color: #fff;
  margin-block-end: 0.3em;
}

h2 {
  color: #fff;
  font-size: 2em;
  font-weight: 500;
  margin-block-end: 0.5em;
}

h1 {
  color: #f9ba47;
  font-size: 2.5em;
  font-weight: 600;
  margin-top: -0.3em;
}
</style>
