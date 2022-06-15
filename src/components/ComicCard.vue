<template>
    <div class="comic">
      <img :src="info.thumb" :alt="info.series">
      <h5>{{ info.series }}</h5>
    </div>
</template>

<script>
export default {
  name: 'ComicCard',
  props: {
    info: Object
  }
}
</script>

<style scoped lang="scss">
.comic {
  margin: 10px;
  width: 15%;
  img {
    width: 100%;
  }
  h5 {
    color: white;
  }
}
</style>