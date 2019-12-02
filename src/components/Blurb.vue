<template>
  <div class="blurb-container">
      <span class="blurb">
        Someone once told me the key to a good website is a nice typeface, some heavy white space, and a touch of color.*
        <br>
        <br>
        I am a UX Designer @ Google and studied ID @ RISD.
        Eventually this site will be cool and quirky but until then this will have to do.
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
        src: url('/assets/monument-grotesk-regular');
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
</style>