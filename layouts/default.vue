<template>
  <div>
    <TheHeader @sidenavToggle="displaySideNav = !displaySideNav" />
    <TheSideNav :show="displaySideNav" @close="displaySideNav = false" />

    <Nuxt />
  </div>
</template>


<script>
import TheHeader from "@/components/Navigation/TheHeader";
import TheSideNav from "@/components/Navigation/TheSidenav";
export default {
  components: {
    TheHeader,
    TheSideNav
  },
  data() {
    return {
      displaySideNav: false
    };
  }
};
</script>

<style>
html {
  font-family: "Open Sans", sans-serif;
}

body {
  margin: 0;
}
</style>
