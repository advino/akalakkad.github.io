<template>
  <div id="app">
    <div class='container'>
      <Test></Test>
      <Thing></Thing>
      <Something></Something>
    </div>
  </div>
</template>

<script>
  import Test from '@/components/Test';
  import Thing from '@/components/Thing';
  import Something from '@/components/Something';

  export default {
    name: 'app',
    components: {
      Test,
      Thing,
      Something
    }
}
</script>

<style>

body {
  width: 100%;
  height: 100vh;
  margin: 0;
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

.container {
  width: 30%;
  text-align: left;
}
</style>
