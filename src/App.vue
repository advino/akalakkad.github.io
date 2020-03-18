<template>
  <div id="app">
   <div class="wrapper">
     <Title></Title>
     <br>
     <Blurb></Blurb>
     <br>
     <br>
    <div class="work-container">
      <h2 class="work-header">Selected Work</h2>
      <div v-for="w in work" :key="w.title" class="workitem-wrapper">
        <WorkItem :title="w.title" :date="w.date"></WorkItem>
      </div>
      
    </div>

   </div>

   <Sketch></Sketch>
  </div>
</template>

<script>
  import Blurb from "@/components/Blurb";
  import Title from '@/components/Title';
  import WorkItem from '@/components/WorkItem';
  import Sketch from '@/components/Sketch';

  export default {
    name: 'app',
    components: {
      Blurb, Title, Sketch, WorkItem
    },
    data() {
      return {
        work: [
          {
            title: "Mixed Signals",
            date: 2020
          },
          {
            title: "OP-5",
            date: 2020
          },
          {
            title: "Album Art Music Player",
            date: 2019
          },
          {
            title: "Vanguard",
            date: 2019
          },
          {
            title: "When is Advait and Asshole?",
            date: 2019
          },
          {
            title: "Text 2 UI",
            date: 2019
          },
          {
            title: "Overlaying Realities",
            date: 2018
          }
        ]
      }
    }
}
</script>

<style>
html,body {
  width: 100%;
  height: 100%;
  min-height: 100%;
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
  box-sizing: border-box;
}

.work-header {
  font-size: 28px;
  font-family: Arimo;
  font-weight: 500;
}

</style>
