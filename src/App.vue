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
  </div>
</template>

<script>
  import Blurb from "@/components/Blurb";
  import Title from '@/components/Title';
  import Links from '@/components/Links';

  export default {
    name: 'app',
    components: {
      Blurb, Title, Links      
    }
}
</script>

<style>
html,body {
  width: 100%;
  height: 100%;

  padding: 0;
  margin: 0;
  box-sizing: border-box;

}

.wrapper {
  width: 70%;
  box-sizing: border-box;
}

#app {
  width: 100%;
  height: 100%;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: flex;
  justify-content: center;
  align-items: center;

  box-sizing: border-box;
}

</style>
