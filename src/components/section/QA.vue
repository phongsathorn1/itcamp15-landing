<template>
  <section class="home-section" id="qa">
    <div class="strip-top"></div>
    <div class="strip-bottom"></div>
    <div class="container">
      <h1 class="text-center">คำถามที่พบบ่อย</h1>
    </div>
  </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
#qa{
  padding: 100px 0px;
  background: #ebebeb;
}
#qa .strip-top{
    background: #ebebeb;
    width: 100%;
    height: 50%;
    position: absolute;
    top: -45px;
    transform: skewY(3deg);
    z-index: 99;
}

#qa .strip-bottom{
    background: #ebebeb;
    width: 100%;
    height: 50%;
    position: absolute;
    bottom: -45px;
    transform: skewY(-3deg);
    z-index: 99;
}
</style>
