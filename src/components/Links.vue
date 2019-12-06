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
        src: url('../assets/fonts/monument-grotesk-regular.otf') format('otf');
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

   @media (max-width: 499px) {
       a {
           width: 100%;
           font-size: 16px;
           display: block;
       }

       .links-container {
           display: block;
       }
   }

   @media (min-width: 500px) {
        a {
            font-size: 24px;
        }
    }

    @media (min-width: 600px) {
        a {
            font-size: 26px;
        }
    }

    @media (min-width: 700px) {
        a {
            font-size: 30px;
        }
    }

    @media (min-width: 800px) {
        a {
            font-size: 33px;
        }
    }
</style>