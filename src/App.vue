<template>
  <div id="app">
    <Heading/>
  </div>
</template>

<script>

import Heading from '@/components/section/Heading.vue'
export default {
  name: 'app',
  components: {
    Heading
  }
}
</script>

<style lang="scss">
body {
  font-family: "Athiti", sans-serif;
  margin: 0;
  padding: 0;
}
</style>
