<template>
  <div class="title-container">
      <span class="title">
         ADVAIT KALAKKAD*
      </span>
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
        src: url('/assets/monument-grotesk-regular.otf') format('otf');
    }

    .title-container {
        width: 100%;
        height: auto;
    }

    .title {
        font-size: 46px;
        font-family: Monument Grotesk;
        line-height: 58px;
    }

       @media (max-width: 599px) {
        .title {
            font-size: 32px;
        }
    }

    @media (min-width: 600px) {
        .title {
            font-size: 38px;
        }
    }

    @media (min-width: 700px) {
        .title {
            font-size: 42px;
        }
    }

     @media (min-width: 800px) {
        .title {
            font-size: 46px;
        }
    }
</style>