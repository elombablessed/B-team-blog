<template>
  <div>
    <TheHeader @sidenavToggle="displaySidenave = !displaySidenave"/>
    <TheSidenav :show="displaySidenave" @close="displaySidenave = false"/>
    <Nuxt />
  </div>
</template>

<script>
export default {
  data(){
    return{
      displaySidenave: false
    }
  }
}
</script>

<style>
html {
    font-family:'Source Sans Pro', sans-serif;
    }
body{
  margin: 0;
}
</style>
