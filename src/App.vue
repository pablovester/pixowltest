<template>
  <div id="app">
    <Bar/>
    <MainHeader/>
    <Section/>
    <Section/>
  </div>
</template>

<script>
import Bar from './components/Bar.vue'
import MainHeader from './components/MainHeader.vue'
import Section from './components/Section.vue'


export default {
  name: 'app',
  components: {
    Bar,
    MainHeader,
    Section
  }
}
</script>

<style>
  #app {
    font-family: 'Montserrat', sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    margin: 0;
    background-color: black;
  }

  body {
    margin: 0;
  }

  h1 {
    font-weight: 700;
  }

  h3, li {
    font-weight: 500;
  }
  .nomargin {
      margin: 0;
    }

  .white {
      color: white;
  }

  div#content.section:nth-of-type(2n+1){
    background-color: #151619;
    min-height: 200vh;
    overflow: hidden;
    clip-path: polygon(0 0, 100% 10%, 100% 90%, 0 100%);
    display: flex;
    justify-content: center;
    align-items: center;
  }

  div#content.section:nth-of-type(2n){
    min-height: 200vh;
    display: flex;
    flex-direction: row-reverse;
    justify-content: center;
    align-items: center;
    margin-left: 5%;
  }

  div#content.section:nth-of-type(2n) img {
    background-image: url("/assets/img3.png");
  }
</style>
