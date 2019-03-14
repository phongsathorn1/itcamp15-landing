<template>
  <section class="home-section" id="about">
    <div class="box-bg">
      <div class="box-bg-wrapper">
        <div class="box-2">
          <div class="box-3"></div>
        </div>
      </div>
    </div>
    <div class="container text-center">
      <span class="subhead">เรื่องราวแห่ง ITCAMP ครั้งที่ 15</span>
      <h1>ปฐมบทแห่งมนตรา</h1>
      <div class="about-wrapper">
        <p>การสร้างสรรค์ “Content” หรือ “เนื้อหา” ถือเป็นหัวใจสำคัญของการทำเว็บ เพราะเนื้อหาที่ดี จะสร้างคุณค่าและความน่าสนใจให้กับเว็บของพวกเรา สาขานี้เหมาะกับน้อง ๆ ที่รักในการเขียน การเล่าเรื่อง และการใช้ภาษา ให้เทพ Apollo ผู้เก่งกาจ เป็นตัวแทนของเหล่านักเขียนคนเก่ง มาเอาชนะใจผู้อ่านให้จงได้!</p>
        <p>ไอทีแคมป์ หรือค่ายปฏิบัติการไอที เป็นค่ายที่จัดขึ้นโดย
        คณะเทคโนโลยีสารสนเทศ สถาบันพระจอมเกล้าเจ้าคุณทหารลาดกระบัง
        เพื่อส่งเสริมอะไรบลาๆก็ว่ากันไป </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
#about{
  min-height: calc(100vh - 100px);
  background-image: linear-gradient(to bottom, #17013c, #22002b);
  color: #ffffff;
  padding-bottom: 150px;
  padding-top: 50px;
}

#about .container{
  position: relative;
  padding-top: 150px;
  padding-bottom: 4vh;
}

#about .about-wrapper{
  padding: 50px 0px;
  width: 55%;
  margin: auto;
  font-family: 'Sarabun', sans-serif;
  font-weight: 100;
  line-height: 44px;
}

.box-bg{
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
  padding: 30px 0px;
}

.box-bg-wrapper{
  margin: auto;
  margin-top: 100px;
  width: 500px;
  height: 500px;
  border: 0.5px solid #555;
  padding: 2em;
  transform: rotate(45deg);
}

// @media (min-width: 1200px){
//   .box-bg-wrapper {
//     max-width: 600px;
//     max-height: 600px;
//   }
// }

@media (max-width: 768px){
  #about .about-wrapper{
    width: auto;
    padding-left: 20px;
    padding-right: 20px;
  }

  .box-bg-wrapper {
    width: 100vh;
    height: 100vh;
  }
}

.box-2 {
  border: 0.5px solid #444;
  width: 100%;
  height: 100%;
}

.box-3 {
  margin: 2em;
  width: calc(100% - 4em);
  height: calc(100% - 4em);
  border: 0.5px solid #222;
}
</style>
