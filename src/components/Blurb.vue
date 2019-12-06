<template>
  <div class="blurb-container">
      <span class="blurb">
        Someone once told me the keys to a good website are a nice typeface, some heavy white space, and a touch of color.*
        <br>
        <br>
        I am a UX Designer @ Google and got my BFA in Industrial Design @ RISD.
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
        src: url('~@/assets/fonts/monument-grotesk-regular.otf') format('font-opentype');
    }

    .blurb-container {
        width: 100%;
        height: auto;
    }

    .blurb {
        width: 100%;
        font-size: 44px;
        font-family: Monument Grotesk;
        /* line-height: 58px; */
    }

    @media (max-width: 599px) {
        .blurb {
            font-size: 30px;
        }
    }

    @media (min-width: 600px) {
        .blurb {
            font-size: 36px;
        }
    }

    @media (min-width: 700px) {
        .blurb {
            font-size: 40px;
        }
    }

     @media (min-width: 800px) {
        .blurb {
            font-size: 44px;
        }
    }

</style>