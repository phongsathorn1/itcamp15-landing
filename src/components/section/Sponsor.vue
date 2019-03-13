<template>
  <div id="sponsor-container">
    <p>สนับสนุนโดย</p>
    <div class="sponsor-row">
      <div class="sponsor-lv1"></div>
      <div class="sponsor-lv1"></div>
      <div class="sponsor-lv1"></div>
    </div>
    <div class="sponsor-row">
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
    </div>
  </div>
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
}

.sponsor-row {
  display: flex;
  justify-content: center;
  margin-top: 6.5em;
}

.sponsor-lv1 {
  width: 131px;
  height: 131px;
  margin: 0 3em;
  transform: rotate(45deg);
  border: solid 3px #ffffff;
}

.sponsor-lv2 {
  width: 100px;
  height: 100px;
  margin: 0 2.5em;
  transform: rotate(45deg);
  border: solid 3px #ffffff;
}

p {
  color: #fff;
  text-align: center;
  font-size: 1.3em;
}
</style>
