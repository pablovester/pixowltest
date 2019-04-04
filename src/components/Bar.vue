<template>
  <div id="bar">
  	<div id="btn">{{ btntxt }}</div>
  </div>
</template>

<script>
export default {
	data () {
		return {
			btntxt: "DOWNLOAD"
		}
	}
}
</script>

<style>
#bar {
  height: 20px;
  width: 100%;
  background-color: rgb(21, 22, 25);
  height: 60px;
  display: flex;
  align-items: center;
  justify-content: center;
}

#btn {
  border-radius: 10px;
  background-color: rgb(58, 190, 239);
  width: 160px;
  height: 40px;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: 800;
}
</style>