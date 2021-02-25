<template>
  <div class="box-unscoped"></div>
  <div class="box-scoped"></div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style>
.box-unscoped {
  width: 2em;
  height: 2em;
  background: #f00;
  animation: rotate-unscoped 2s linear infinite;
}

@keyframes rotate-unscoped {
  100% {
    transform: rotate(1turn);
  }
}
</style>

<style scoped>
.box-scoped {
  width: 2em;
  height: 2em;
  background: #0f0;
  animation: rotate-scoped 2s linear infinite;
}

@keyframes rotate-scoped {
  100% {
    transform: rotate(1turn);
  }
}
</style>
