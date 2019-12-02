<template>
  <div class="links-container">
      <a href="https://www.are.na/advait-kalakkad">Are.na  ↗</a>
      <a href="https://github.com/akalakkad">Github  ↗</a>
      <a href="https://twitter.com/computerpolygl1">Twitter  ↗</a>
      
  </div>
</template>

<script>
export default {

}
</script>

<style>

    @font-face {
        font-family: Prophet;
        src: url('/assets/Prophet.otf');
    }  

    @font-face {
        font-family: Monument Grotesk;
        src: url('/assets/monument-grotesk-regular');
    }

    .links-container {
        width: 100%;
        height: auto;
        display: flex;
        justify-content: space-between;
    }

    a {
        width: 25%;
        border-style: solid;
        border-width: 2px;
        border-radius: 60px;
        padding: 8px;
        
        font-family: Monument Grotesk;
        font-size: 33px;
        color: black;
        text-decoration: none; 
        text-align: center;

    }

    span {
        text-decoration: none;
    }
</style>