<template>
  <div>

  </div>

</template>


<script>
  import p5 from 'p5/lib/p5.js';
  export default {

    mounted(p5) {
      p5.setup = () => {
        p5.createCanvas(500,500);
        p5.ellipse(p5.width/2, p5.height/2, 50,50)
      }
    }
  }
</script>

<style>



</style>
