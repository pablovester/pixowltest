<template>
  <div id="app">
    <Bar/>
    <MainHeader/>
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
</style>
