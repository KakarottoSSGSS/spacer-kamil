<template>
    <div class="heroImage"></div>
</template>

<script>
export default {
    name: heroImage,
}
</script>

<style lang="scss" scoped>
 .heroImage {
  width:  100%;
  height: 100vh;
  top: 0;
  z-index: -1;
  position: fixed;
  background-image: url('../assets/heroimage.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position:  80% 0%;

 }

 .heroImage::after{
     content: '';
     position: absolute;
     top: 0;
     left: 0;
     z-index: 1;
     width: 100%;
     height: 100vh;
     background: rgba(0, 0, 0, .2);


 }
</style>

