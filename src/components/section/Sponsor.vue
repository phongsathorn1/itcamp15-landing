<template>
  <lazy-component>
    <div id="sponsor-container">
      <p>สนับสนุนโดย</p>
      <div class="sponsor-row">
        <div class="sponsor-lv1">
          <img
            src="@/assets/sponsor/it.png"
            alt="คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง"
          >
        </div>
        <div class="sponsor-lv1">
          <img src="@/assets/sponsor/kmitl.svg" alt="สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง" />
        </div>
        <!-- <div class="sponsor-lv1"></div>
        <div class="sponsor-lv1"></div>-->
      </div>
      <!-- <div class="sponsor-lv1"></div>
      <div class="sponsor-lv1"></div> -->
    </div>
    <!-- <div class="sponsor-row">
      <div class="sponsor-lv2"></div>
      <div class="sponsor-lv2"></div>
      <div class="sponsor-lv2"></div>
      <div class="sponsor-lv2"></div>
      <div class="sponsor-lv2"></div>
    </div>
    <div class="sponsor-row">
      <div class="sponsor-lv2"></div>
      <div class="sponsor-lv2"></div>
      <div class="sponsor-lv2"></div>
      <div class="sponsor-lv2"></div>
      </div>-->
  </lazy-component>
</template>
<script>
export default {
  name: 'Sponsor'
}
</script>

<style lang="scss" scoped>
#sponsor-container {
  background-image: linear-gradient(to top, #000000, rgba(0, 0, 0, 0));
  width: 100%;
  padding-bottom: 5em;
  position: relative;
  z-index: 100;
}

.sponsor-row {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

.sponsor-row img {
  display: block;
  width: 100%;
}

.sponsor-lv1 {
  width: 131px;
  height: 131px;
  margin: 0 30px;
}

.sponsor-lv2 {
  width: 100px;
  height: 100px;
  margin: 0 2.5em;
}

p {
  color: #fff;
  text-align: center;
  font-size: 1.3em;
}
</style>
