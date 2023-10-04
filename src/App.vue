<template>
  <div 
  :data-device="deviceType"
  class="wrapper"
  >
  <Navbar />
  </div>
</template>


<script>
import Navbar from './components/Navbar/Navbar.vue';
import LandingHeader from './components/LandingHeader/LandingHeader.vue';

export default {
  components: {
    Navbar,
    LandingHeader,
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
