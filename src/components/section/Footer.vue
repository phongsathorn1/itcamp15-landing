<template>
  <section class="home-section" id="timeline">
    <!-- <div class="strip-top"></div> -->
    <footer class="page-footer font-small blue">
      <!-- Copyright -->
      <div class="footer-copyright text-center py-3">
        © 2019 Copyright: ITForge
      </div>
      <!-- Copyright -->
    </footer>
  </section>
</template>

<script>
export default {};
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

.timeline-icon {
  height: 150px;
  width: 150px;
  transform: rotate(45deg);
  overflow: hidden;
  text-align: center;
  margin: auto;
}

.timeline-icon-img {
  transform: rotate(-45deg);
  display: block;
  margin: auto;
}
</style>
