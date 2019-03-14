<template>
    <section class="home-section" id="timeline">
        <div class="strip-top"></div>
        <div class="strip-bottom"></div>
        <div class="container">
            <h1>กำหนดการ</h1>
            <span class="subhead">ตารางเวลาของค่ายไอทีแคมป์</span>
            <div class="timeline-wrapper">
                <div class="row">
                    <div class="col-md-3 timeline-block">
                        <div class="temp-block">
                        </div>
                        <div class="timeline-title">
                            รับสมัครค่าย
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 30 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3 timeline-block">
                        <div class="temp-block">
                        </div>
                        <div class="timeline-title">
                            รับสมัครค่าย
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 30 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3 timeline-block">
                        <div class="temp-block">
                        </div>
                        <div class="timeline-title">
                            รับสมัครค่าย
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 30 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3 timeline-block">
                        <div class="temp-block">
                        </div>
                        <div class="timeline-title">
                            รับสมัครค่าย
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 30 เมษายน
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
#timeline .subhead{
    color: #242424;
    font-size: 25px;
}

#timeline{
    background: #ebebeb;
}

#timeline .strip-top{
    background: #ebebeb;
    width: 100%;
    height: 50%;
    position: absolute;
    top: -45px;
    transform: skewY(3deg);
    z-index: 99;
}

#timeline .strip-bottom{
    background: #ebebeb;
    width: 100%;
    height: 50%;
    position: absolute;
    bottom: -45px;
    transform: skewY(-3deg);
    z-index: 99;
}

#timeline .container{
    position: relative;
    z-index: 100;
}

#timeline .timeline-wrapper{
    padding: 50px 0px;
    text-align: center;
}
#timeline .timeline-wrapper .timeline-title{
    font-size: 30px;
    color: #eea113;
    margin-top: 50px;
}

#timeline .timeline-wrapper .timeline-range{
    font-size: 25px;
    color: #242424
}

#timeline .timeline-block{
    margin-bottom: 30px;
}

.temp-block{
    height: 200px;
    width: 100%;
    background: #242424;
}
</style>
