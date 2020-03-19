<template>
  <div id="app">
   <div class="wrapper">
     <Title></Title>
     <br>
     <Blurb></Blurb>
     <br>
     <br>
    <div class="work-container">
      <h2 class="work-header">SELECTED WORK</h2>
      <div v-for="w in work" :key="w.title" class="workitem-wrapper">
        <WorkItem :title="w.title" :date="w.date"></WorkItem>
      </div>
    </div>
    <div class="work-container">
      <h2 class="work-header">OTHER</h2>
      <div v-for="w in other" :key="w.title" class="workitem-wrapper">
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
            title: "Bad Design is Good Design When You Use AI",
            date: 2019
          },
          {
            title: "When is Advait an Asshole?",
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
        ],
        other: [
          {
            title: "A Window to Look Somwhere Else",
            date: 2020
          },
          {
            title: "My Dog Ate My Image Classifier",
            date: 2019
          }
        ]
      }
    }
}
</script>

<style>

@font-face {
  font-family: 'Whyte Inktrap';
  src: url('~@/assets/fonts/WhyteInktrap-Medium.woff');
  font-weight: medium;
}

@font-face {
  font-family: 'Whyte Inktrap';
  src: url('~@/assets/fonts/WhyteInktrap-Regular.woff2');
  font-weight: normal;
}


@font-face {
  font-family: 'Whyte';
  src: url('~@/assets/fonts/Whyte-Book.woff2');
  font-weight: normal;
}


@font-face {
  font-family: 'Whyte';
  src: url('~@/assets/fonts/Whyte-Light.woff');
  font-weight: light;
}


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

.work-container {
  margin-bottom: 60px;
}

.work-header {
  font-size: 14px;
  font-family: Whyte Inktrap;
  font-weight: medium;
  letter-spacing: 1px;
}

</style>
