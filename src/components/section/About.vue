<template>
  <div id="about-container">
    <div id="about-box">
      <div id="box-2">
        <div id="box-3"></div>
      </div>
    </div>
    <div id="about-content">
      <h3>เรื่องราวแห่ง ITCAMP ครั้งที่ 15</h3>
      <h2>ปฐมบทแห่งมนตรา</h2>
      <p
        id="about-justify"
      >การสร้างสรรค์ “Content” หรือ “เนื้อหา” ถือเป็นหัวใจสำคัญของการทำเว็บ เพราะเนื้อหาที่ดี จะสร้างคุณค่าและความน่าสนใจให้กับเว็บของพวกเรา สาขานี้เหมาะกับน้อง ๆ ที่รักในการเขียน การเล่าเรื่อง และการใช้ภาษา ให้เทพ Apollo ผู้เก่งกาจ เป็นตัวแทนของเหล่านักเขียนคนเก่ง มาเอาชนะใจผู้อ่านให้จงได้!</p>
      <p>
        <b>ไอทีแคมป์ หรือค่ายปฏิบัติการไอที</b> เป็นค่ายที่จัดขึึ้นโดย
        <br>คณะเทคโนโลยีสารสนเทศ สถาบันพระจอมเกล้าเจ้าคุณทหารลาดกระบัง
        <br>เพื่อส่งเสริมอะไรบลาๆก็ว่ากันไป
      </p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
#about-container {
  width: 100%;
  background-image: linear-gradient(to bottom, #17013c, #22002b);
  padding: 15vw 0;
  min-height: 750px;
  display: flex;
  justify-content: center;
  align-items: center;
}

#about-box {
  position: absolute;
  margin: 0 auto;
  width: 45vw;
  height: 45vw;
  max-width: 450px;
  max-height: 450px;
  border: 0.5px solid #555;
  padding: 2em;
  transform: rotate(45deg);
  z-index: 2;
}

#box-2 {
  border: 0.5px solid #444;
  width: 100%;
  height: 100%;
}

#box-3 {
  margin: 2em;
  width: calc(100% - 4em);
  height: calc(100% - 4em);
  border: 0.5px solid #222;
}

#about-content {
  position: absolute;
  width: 100%;
  max-width: 1200px;
  text-align: center;
  color: white;
  z-index: 3;

  h3 {
    font-weight: 200;
    margin-bottom: 1em;
  }

  h2 {
    color: #eea113;
    font-size: 2.5em;
    font-weight: 500;
    margin-bottom: 1em;
  }

  p {
    width: 47%;
    margin: 0 auto 2em auto;
    font-weight: 200;
  }

  b {
    font-weight: 400;
  }
}

#about-justify {
  text-align: justify;
}
</style>
