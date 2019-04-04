<template>
  <div>
    <h1>{{ msg }}</h1>
    <img src="../assets/bannerimg.png">
    <h1 class="nomargin">{{title}}</h1>
    <h3>{{subtitle}}</h3>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: "CREATE. ANIMATE. PLAY.",
      subtitle: "VoxEditor is the first software that allows you to create your own voxel models, rig them and animate them in no time."
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

* {
  text-align: center;
}
h1 {
  font-size: 105px;
  background: -webkit-linear-gradient(#ff9626, #fe6920);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}

h3{
  margin: 0 5% 0 5%;
  font-size: 24px;
  color: #ffff;
  margin-bottom: 5%;
}
img {
  width: 80%;
}
</style>
