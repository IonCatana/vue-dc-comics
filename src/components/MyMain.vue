//HTML 
<template>
  <div id="app">
    <div class="contents">
      <h1 v-for="(link, i) in links" :key="i">
        {{ link.text }}
      </h1>
    </div>
  </div>
</template>

// JS script Vue
<script>
export default {
  name: "MyMain",
  data() {
    return {
      links: [
        {
          text: "--> Contents goes here <--",
        },       
      ],
    };
  },
};
</script>

// Style CSS
<style lang="scss" scoped>
#app {
  width: 100vw;
  background-color: #1c1c1c;
  color: white;
}
.contents {
  width: 70%;
  margin: 0 auto;
}
</style>