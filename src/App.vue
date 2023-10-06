<template>
  <!-- <div 
  :data-device="deviceType"
  class="wrapper"
  >
  <Navbar />
  </div> -->
<div class="wrapper">
  <Test />
</div>
</template>


<script>
import Navbar from './components/Navbar/Navbar.vue';
import LandingHeader from './components/LandingHeader/LandingHeader.vue';
import Test from './components/test/test.vue';

export default {
  components: {
    Navbar,
    LandingHeader,
    Test
  },

  data() {
    return {
      deviceType: '', // Initialize deviceType
    };
  },
  watch: {
    // Watch the window.innerWidth property for changes
    '$options.methods.checkDeviceWidth': 'checkDeviceWidth',
  },
  methods: {
    checkDeviceWidth() {
      // Check the viewport width and update deviceType accordingly
      this.deviceType = window.innerWidth < 1024 ? 'mobile' : 'desktop';
    },
  },
  mounted() {
    // Initial check and watch for changes in viewport width
    this.checkDeviceWidth();
    window.addEventListener('resize', this.checkDeviceWidth);
  },
  beforeDestroy() {
    // Remove the event listener when the component is destroyed to prevent memory leaks
    window.removeEventListener('resize', this.checkDeviceWidth);
  },
};
</script>

<style lang="scss">
.wrapper {
  display: flex;
  padding: 1.5rem;
  justify-content: center;
  align-items: flex-start;
  align-content: flex-start;
  gap: 1.5rem;
  flex: 1 0 0;
  flex-wrap: wrap;
}
</style>
