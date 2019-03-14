<template>
  <div id="app">
    <Heading/>
    <About/>
    <Registration/>
    <Timeline/>
    <Location/>
    <QA/>
    <Gallery/>
  </div>
</template>

<script>
import Heading from '@/components/section/Heading.vue'
import About from '@/components/section/About.vue'
import Registration from '@/components/section/Registration.vue'
import Timeline from '@/components/section/Timeline.vue'
import Location from '@/components/section/Location.vue'
import QA from '@/components/section/QA.vue'
import Gallery from '@/components/section/Gallery.vue'

export default {
  name: 'app',
  components: {
    Heading,
    About,
    Registration,
    Timeline,
    Location,
    QA,
    Gallery
  }
}
</script>

<style lang="scss">
body {
  font-family: "Athiti", sans-serif;
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}

.home-section h1{
  color: #eea113;
  font-size: 50px;
}

.home-section{
  padding: 25px 0px;
  font-size: 1.2em;
  position: relative;
}

.home-section .subhead{
  display: block;
}

.ractangle-top-1{
  background: #FFF;
  height: 100px;
}
</style>
