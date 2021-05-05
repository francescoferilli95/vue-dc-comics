<template>
  <div class="box">
      <img :src="details.thumb" :alt="details.series">
      <p>{{details.series}}</p>
  </div>
</template>

<script>
export default {
    name: 'Comics',
    props: ['details']
}
</script>

<style scoped lang="scss">

.box {
    flex-basis: calc(100% / 6);
    img {
        width: 50%;
        margin-top: 5px;
        margin-bottom: 5px;
    }
    p {
        margin-bottom: 20px;
    }
}

</style>