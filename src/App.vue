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
</style>
