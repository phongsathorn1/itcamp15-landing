<template>
    <section class="home-section" id="location">
        <div class="hover-dark-bg"></div>
        <div class="container">
            <h1 class="text-right">สถานที่จัดค่าย</h1>
            <span class="subhead text-right">คณะเทคโนโลยีสารสนเทศ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง</span>
            <div class="row location-wrapper">
                <div class="col-md-5">
                    <ul class="transportation-list">
                        <li>
                            <div class="li-head">เดินทางโดยรถเมล์</div>
                            รถประจำทางที่ผ่าน สาย 51, 52, 150, 356, ปอ.150, ปอ.166
                        </li>
                        <li>
                            <div class="li-head">เดินทางโดยรถเมล์</div>
                            รถประจำทางที่ผ่าน สาย 51, 52, 150, 356, ปอ.150, ปอ.166
                        </li>
                        <li>
                            <div class="li-head">เดินทางโดยรถเมล์</div>
                            รถประจำทางที่ผ่าน สาย 51, 52, 150, 356, ปอ.150, ปอ.166
                        </li>
                    </ul>
                </div>
                <div class="col-md-7">
                    <div class="embed-responsive embed-responsive-16by9">
                        <iframe class="embed-responsive-item" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1056.6441030332855!2d100.77986334916747!3d13.731297018707501!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0xcb43a76f038c38ca!2z4LiE4LiT4Liw4LmA4LiX4LiE4LmC4LiZ4LmC4Lil4Lii4Li14Liq4Liy4Lij4Liq4LiZ4LmA4LiX4LioIOC4quC4luC4suC4muC4seC4meC5gOC4l-C4hOC5guC4meC5guC4peC4ouC4teC4nuC4o-C4sOC4iOC4reC4oeC5gOC4geC4peC5ieC4suC5gOC4iOC5ieC4suC4hOC4uOC4k-C4l-C4q-C4suC4o-C4peC4suC4lOC4geC4o-C4sOC4muC4seC4hw!5e0!3m2!1sth!2sth!4v1552574555073" frameborder="0" style="border:0" allowfullscreen></iframe>
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

<style lang="scss" scoped>
#location{
    color: #ffffff;
    padding: 150px 0px;
    background-image: url(../../assets/location-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}

#location .stripe{
    transform: skewY(6deg);
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0px;
}

#location .container{
    position: relative;
    z-index: 3;
}

#location h1{
    text-align: right;
}
#location .li-head{
    font-weight: bold;
}

#location .transportation-list{
    list-style: none;
}

#location .transportation-list li{
    margin-bottom: 20px;
}

#location .location-wrapper{
    padding: 50px 0px;
}

#location .hover-dark-bg{
    background: rgba(0, 0, 0, 0.81);
    height: 100%;
    width: 100%;
    top: 0px;
    position: absolute;
    z-index: 2;
}
</style>
