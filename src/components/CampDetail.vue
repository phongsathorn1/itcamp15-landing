<template>
  <div class="camp-detail-box" :style="{ borderColor: color }">
    <div class="d-flex justify-content-start align-items-center">
      <div class="col-2 d-none d-sm-block">
        <div class="camp-detail-logo">
          <img :src="require(`@/assets/camp/${logo}`)" />
        </div>
      </div>
      <div class="col-10">
        <h2 :style="{ color: color }">{{campname}}</h2>
        <a class="btn btn-register" :style="{ borderColor: color, color: color}" :href="`https://register.itcamp.in.th/${id}`">สมัครค่าย {{campname}}</a>
      </div>
    </div>
    <div class="row">
      <div class="col-12">
        <div class="inner-camp-detail-box">
          <p v-html="detail"></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["id", "logo", "campname", "detail", "color"]
}
</script>


<style lang="scss" scoped>
.camp-detail-box{
  border: 2px solid #000;
  border-radius: 5px;
  padding: 20px;
}

.camp-detail-logo img{
  display: block;
  width: 100%;
}

.inner-camp-detail-box{
  margin-top: 20px;
}

.camp-detail-box .btn-register{
  // background: linear-gradient(243deg, #fad961, #f76b1c);
  font-size: 1em;
  font-weight: 500;
  color: #ffffff;
  border: 2px solid transparent;
}

.camp-detail-box .btn-register:hover{
  background: #ccc;
}

.inner-camp-detail-box p{
  text-indent: 2em;
}
</style>
