<template>
  <section class="home-section" id="qa">
    <div class="strip-top"></div>
    <div class="strip-bottom"></div>
    <div class="container">
      <h1 class="text-center">คำถามที่พบบ่อย</h1>
      <div class="qa-wrapper">
        <ul class="qa-list">
          <li>
            <div class="qa-question">
              ใครสมัครค่ายนี้ได้บ้าง?
            </div>
            <div class="qa-answer">
              <u><b>ตอบ</b></u> น้องๆ ที่<u><b>กำลัง</b></u>ศึกษาในระดับชั้น ม.4 ถึง ม.6 และน้องๆ ที่ศึกษา ปวช. ปวส. หรือเทียบเท่า
            </div>
          </li>
        </ul>
      </div>
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

#qa .container{
  position: relative;
  z-index: 100;
}
</style>
