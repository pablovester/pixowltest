<template>
  <div id="bar">
  	<div id="btn">{{ btntxt }}DOWNLOAD</div>
  </div>
</template>

<script>
data: {
  btntxt: "boke"
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