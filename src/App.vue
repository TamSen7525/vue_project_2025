<template>
  <!-- Task 1 -->
  <div>
    <h1>Task 1</h1>
    <p>{{ obj.x + obj.y + obj.z }}</p>

  </div>
</template>

<script>
export default {
  data() {
	return {
		obj: {x: 1, y: 2, z: 3},
	}
}
}
</script>

<style scoped>

div {
  margin-bottom: 20px;
}

h1 {
  margin: 0 0 10px 0;
}

p {
  margin: 5px 0;
}
</style>