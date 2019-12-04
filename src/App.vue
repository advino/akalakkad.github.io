<template>
  <div id="app">
   <div class="wrapper">
     <Title></Title>
     <br>
     <Blurb></Blurb>
     <br>
     <br>
     <Links></Links>
   </div>

   <Sketch></Sketch>
  </div>
</template>

<script>
  import Blurb from "@/components/Blurb";
  import Title from '@/components/Title';
  import Links from '@/components/Links';
  import Sketch from '@/components/Sketch';

  export default {
    name: 'app',
    components: {
      Blurb, Title, Links, Sketch
    }
}
</script>

<style>
html,body {
  width: 100%;
  height: 100%;

  padding: 5px;
  margin: 0;
  box-sizing: border-box;

  /* cursor: none; */
}

.wrapper {
  width: 70%;
    margin-top: 40px;
  box-sizing: border-box;
  z-index: 2;
}

#app {
  width: 100%;
  height: 100%;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex;
  justify-content: center;
  /* align-items: center; */
  box-sizing: border-box;
}

</style>
