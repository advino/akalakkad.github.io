<template>
  <div class="blurb-container">
      <span class="blurb">
        Someone once told me the keys to a good website were a nice typeface, some heavy white space, and a touch of color
      </span>
  </div>
</template>

<script>
export default {

}
</script>

<style>

    .blurb-container {
        width: 100%;
        height: auto;
    }

    .blurb {
        width: 100%;
        font-size: 44px;
        font-family: Whyte;
        font-weight: normal;
    }

    @media (max-width: 599px) {
        .blurb {
            font-size: 24px;
            line-height: 28px;
        }
    }

    @media (min-width: 600px) {
        .blurb {
            font-size: 28px;
            line-height: 32px;
        }
    }

    @media (min-width: 700px) {
        .blurb {
            font-size: 32px;
            line-height: 36px;
        }
    }

     @media (min-width: 800px) {
        .blurb {
            font-size: 32px;
            line-height: 38px;
        }
    }

</style>