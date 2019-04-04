<template>
  <div id="content">
    <img src="../assets/img2.png">
    <div class="text-container">
      <h1 class="white">{{title}}</h1>
      <h3>{{info}}</h3>
      <ul>
        <h2 class="title-2 nomargin">{{title2}}</h2>
          <li class="white">All in one software with incredible performance</li>
          <li class="white">Windows and Mac supported</li>
          <li class="white">Amazing voxel creation tools</li>
          <li class="white">Emisive Wand. Make your work glow</li>
          <li class="white">Increase your voxels to get that level of detail</li>
          <li class="white">Work with a big Canvas</li>
          <li class="white">Mirror XYZ. Work less, we take care of the rest</li>
          <li class="white">Voxel, Quads and super fast Render view</li>
          <li class="white">Advanced Color Palette</li>
          <li class="white">Super friendly 3D enviroment to work</li>
          <li class="white">And much more</li>
      </ul>
     </div> 
  </div>
</template>

<script>
export default {
	data () {
		return {
			title: "POWERFUL EASY TO USE MODELING TOOLS",
      info: "Make the most of your creativity with a robust set of tools. If you are an advanced 3D modeler or just starting out, with our super user-friendly interface you will creating amazing stuff right away.",
      title2: "FEATURES"
		}
	}
}
</script>

<style>
#content {
  background-color: #151619;
  min-height: 200vh;
  overflow: hidden;
  clip-path: polygon(0 0, 100% 10%, 100% 90%, 0 100%);
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
<style scoped>
img{
  width: 100%;
}

h1 {
  font-size: 48px;
  margin-bottom: 0;
}

h3 {
  color: #b2b5b7
}

.title-2 {
  font-size: 36px;
  color: #fe6b20;
}

li {
  font-size: 24px;
}

</style>