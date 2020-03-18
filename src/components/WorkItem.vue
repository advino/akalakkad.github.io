<template>
  <div class="workitem-container">
      <h3 class="workitem-title">
          {{ title }}
      </h3>
      <h4 class="workitem-date">
          {{ date }}
      </h4>
  </div>
</template>

<script>
export default {
    components: {},
    props: ['title', 'date'],
    data() {
        return {

        }
    }
}
</script>

<style>
    .workitem-container {
        display: flex;
        width: 100%;
        height: auto;
        justify-content: space-between;
        color: black;
        font-family: Arimo;
        
        font-size: 20px;
    }

    .workitem-container h3, h4 {
        margin: 0;
        margin-bottom: 20px;
        font-weight: normal;
    }

</style>