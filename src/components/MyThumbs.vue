<template>
  <div class="card_wrapper">
    <div class="cards">
      <img :src="thumb" alt="" />
      <h5>{{ series }}</h5>
    </div>    
  </div>
</template>

<script>
export default {
  props: {
    thumb: String,
    series: String,
  },
};
</script>

<style lang="scss" scoped>
img {
  width: 90%;
  height: 90%;
}
h5{
  font-size: 12px;
  text-transform: uppercase;
}

.cards {
  width: 100%;
  height: 100%; 
  aspect-ratio: 1/1;
  
}
.card_wrapper {
  width: calc((100% / 6) - 20px);
  max-height: 180px;  
}
</style>