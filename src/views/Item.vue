<template>
  <div class="container">
    <h1>{{ $route.params.name }}</h1>
    <img :src="$route.params.url" :alt="$route.params.name" />
  </div>
</template>

<script>
export default {
  name: "Item",
};
</script>

<style scoped lang="scss">
.container {
  width: 100%;
  overflow: hidden;
  height: 85vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  h1 {
    width: 100%;
    margin-bottom: 20px;
    text-align: center;
  }

  img {
    width: 340px;
    height: auto;
  }
}
</style>