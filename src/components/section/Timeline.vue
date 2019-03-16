<template>
    <section class="home-section" id="timeline">
        <div class="strip-top"></div>
        <div class="strip-bottom"></div>
        <div class="container">
            <h1>กำหนดการ</h1>
            <span class="subhead">ตารางเวลาของค่ายไอทีแคมป์</span>
            <div class="timeline-wrapper">
                <div class="row">
                    <div class="col-md-3 col-6 timeline-block">
                        <div class="timeline-icon">
                            <img class="timeline-icon-img" src="@/assets/group-7.svg" />
                        </div>
                        <div class="timeline-title">
                            เปิดรับสมัคร
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 16 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3 col-6 timeline-block">
                        <div class="timeline-icon">
                            <img class="timeline-icon-img" src="@/assets/group-6.svg" />
                        </div>
                        <div class="timeline-title">
                            ประกาศผล
                        </div>
                        <div class="timeline-range">
                            28 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3 col-6 timeline-block">
                        <div class="timeline-icon">
                            <img class="timeline-icon-img" src="@/assets/group-5.svg" />
                        </div>
                        <div class="timeline-title">
                            ยืนยันสิทธิ์
                        </div>
                        <div class="timeline-range">
                            26 เมษายน - 3 พฤษภาคม
                        </div>
                    </div>
                    <div class="col-md-3 col-6 timeline-block">
                        <div class="timeline-icon">
                            <img class="timeline-icon-img" src="@/assets/group-4.svg" />
                        </div>
                        <div class="timeline-title">
                            เปิดค่าย
                        </div>
                        <div class="timeline-range">
                            30 พฤษภาคม - 2 มิถุนายน
                        </div>
                    </div>
                </div>
            </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
}
</script>

<style lang="scss">
#timeline {
  background: #ebebeb;
}

#timeline .strip-top {
  background: #ebebeb;
  width: 100%;
  height: 50%;
  position: absolute;
  top: -45px;
  transform: skewY(3deg);
  z-index: 99;
}

#timeline .strip-bottom {
  background: #ebebeb;
  width: 100%;
  height: 50%;
  position: absolute;
  bottom: -45px;
  transform: skewY(-3deg);
  z-index: 99;
}

#timeline .container {
  position: relative;
  z-index: 100;
}

#timeline .timeline-wrapper {
  padding: 50px 0px;
  text-align: center;
}
#timeline .timeline-wrapper .timeline-title {
  font-size: 1.5em;
  color: #eea113;
  margin-top: 50px;
}

#timeline .timeline-wrapper .timeline-range {
  font-size: 1em;
  color: #242424;
}

#timeline .timeline-block {
  margin-bottom: 30px;
}

.timeline-icon{
    height: 150px;
    width: 150px;
    transform: rotate(45deg);
    overflow: hidden;
    text-align: center;
    margin: auto;
}

.timeline-icon-img{
    transform: rotate(-45deg);
    display: block;
    margin: auto;
}
</style>
