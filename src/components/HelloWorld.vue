<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <img src="../assets/bannerimg.png">
    <h1>CREATE. ANIMATE. PLAY.</h1>
    <h2>VoxEditor is the first software that allows you to create your own voxel models, rig them and animate them in no time.</h2>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  font-size: 105px;
  font-weight: 700;
  background: -webkit-linear-gradient(#ff9626, #fe6920);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
h2{
  font-size: 18px;
  font-weight: 500;
  color: #ffff;
}
img {
  width: 80%;
}
</style>
