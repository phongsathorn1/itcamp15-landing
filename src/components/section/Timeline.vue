<template>
    <section class="home-section" id="timeline">
        <div class="container">
            <h1>กำหนดการ</h1>
            <span class="subhead">ตารางเวลาของค่ายไอทีแคมป์</span>
            <div class="timeline-wrapper">
                <div class="row">
                    <div class="col-md-3">
                        <div class="temp-block">
                        </div>
                        <div class="timeline-title">
                            รับสมัครค่าย
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 30 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="temp-block">
                        </div>
                        <div class="timeline-title">
                            รับสมัครค่าย
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 30 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3">
                        <div class="temp-block">
                        </div>
                        <div class="timeline-title">
                            รับสมัครค่าย
                        </div>
                        <div class="timeline-range">
                            15 มีนาคม - 30 เมษายน
                        </div>
                    </div>
                    <div class="col-md-3">
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
.home-section h1{
    color: #eea113;
    font-size: 50px;
}

#timeline.home-section .subhead{
    color: #242424;
    font-size: 25px;
}
#timeline.home-section{
    padding: 30px 0px;
    background: #ebebeb;
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

.temp-block{
    height: 200px;
    width: 100%;
    background: #242424;
}
</style>
