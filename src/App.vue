<template>
  <div class="app">
 
  <router-view />
  <!-- router  view robi to ze jak klikniemyt w router-link about to nas przenosi na component about -->
  </div>
</template>

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css?family=Montserrat:300,400,600,800');

$font-weight-light: 300;
$font-weight-normal: 400;
$font-weight-bold: 600;
$font-weight-black: 800;

* {
  box-sizing: border-box;
}

body {
  font-family: 'Montserrat', sans-serif;
  margin: 0;
  padding: 0;
}

</style>
