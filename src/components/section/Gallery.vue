<template>
  <section class="home-section" id="gallery">
    <div class="container-fluid">
      <h1 class="text-center">ภาพกิจกรรม</h1>
      <div class="gallery-wrapper">
        <lazy-component>
          <slick class="gallery-slider" ref="slick" :options="slickOptions">
            <div class="gallery-item" v-for="image in images" :key="image">
              <img :src="image" alt>
            </div>
          </slick>
        </lazy-component>
      </div>
    </div>
  </section>
</template>

<script>
import Slick from 'vue-slick'
import 'slick-carousel/slick/slick.css'
import 'slick-carousel/slick/slick-theme.css'

export default {
  components: {
    Slick
  },
  data () {
    return {
      images: [
        'images/slide/DSC_4556.jpg',
        'images/slide/IMG_1412.jpg',
        // 'images/slide/LRM_EXPORT_20180604_090735.jpg',
        'images/slide/DSC_5869.jpg',
        'images/slide/IMG_6816.jpg',
        'images/slide/_DSC6401.jpg',
        'images/slide/DSC_6534.jpg',
        'images/slide/IMG_9685.JPG',
        'images/slide/_DSC8423.jpg',
        'images/slide/DSC_7206.jpg',
        'images/slide/IMG_9921.JPG',
        'images/slide/IMG_1363.jpg',
        'images/slide/LRM_EXPORT_20180604_090120.jpg'
      ],
      slickOptions: {
        centerMode: true,
        centerPadding: '20px',
        slidesToShow: 3,
        slidesToScroll: 1,
        autoplay: true,
        autoplaySpeed: 2000,
        responsive: [
          {
            breakpoint: 840,
            settings: {
              arrows: false,
              centerMode: false,
              centerPadding: '40px',
              slidesToShow: 2
            }
          },
          {
            breakpoint: 480,
            settings: {
              arrows: false,
              centerMode: false,
              // centerPadding: '40px',
              slidesToShow: 1
            }
          }
        ]
      }
    }
  },
  beforeUpdate () {
    if (this.$refs.slick) {
      this.$refs.slick.destroy()
    }
  },
  updated () {
    this.$nextTick(function () {
      if (this.$refs.slick) {
        this.$refs.slick.create(this.slickOptions)
      }
    })
  },
  methods: {
    next () {
      this.$refs.slick.next()
    },
    prev () {
      this.$refs.slick.prev()
    },
    reInit () {
      // Helpful if you have to deal with v-for to update dynamic lists
      this.$nextTick(() => {
        this.$refs.slick.reSlick()
      })
    }
  }
}
</script>

<style lang="scss" scoped>
#gallery {
  background: #fbfbfb;
  padding: 100px 0px;
}

#gallery h1 {
  color: #333333;
}

.gallery-slider .slick-slide img {
  width: 100%;
  display: block;
}

.gallery-slider .slick-center .gallery-item {
  transform: scale(1.08);
}

.gallery-slider .gallery-item {
  padding: 3%;
  transition: all 300ms ease;
}

.gallery-wrapper {
  width: 80%;
  margin: 50px auto;
}

@media (max-width: 840px) {
  .gallery-wrapper {
    width: 90%;
  }
}

@media (max-width: 1024px) {
  .gallery-wrapper {
    width: 90%;
  }
}
</style>
