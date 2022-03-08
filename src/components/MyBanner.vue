<template>
  <div id="app">
    <div class="banner_blu">
      <div class="banner_items">
        <ul>
          <li v-for="(link, i) in links" :key="i">
            <a :href="link.href">
              <div class="img_banner">
                <img :src="require('../assets/img/' + link.imgUrl)" />
              </div>
              <h4>{{ link.text }}</h4>
            </a>
          </li>                            
        </ul>
      </div>
    </div>
  </div>
</template>

// JS script Vue
<script>
export default {
  name: "MyBannerBlu",
  data() {
    return {
      links: [
        {
          href: "#",
          imgUrl: "buy-comics-digital-comics.png",
          text: "Digital Comics",
        },
        {
          href: "#",
          imgUrl: "buy-comics-merchandise.png",
          text: "Dc Merchandise",
        },
        {
          href: "#",
          imgUrl: "buy-comics-subscriptions.png",
          text: "Subscriptions",
        },
        {
          href: "#",
          imgUrl: "buy-comics-shop-locator.png",
          text: "Comic Shop Location",
        },
        {
          href: "#",
          imgUrl: "buy-dc-power-visa.png",
          text: "Dc Power Visa",
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
.banner_blu {
  width: 100%;
  height: 150px;
  background-color: #0282f9;
  display: flex;
  align-items: center;
}
.banner_items {
  width: 70%;
  margin: 0 auto;
  display: flex;
}
.img_banner {
  margin-right: 10px;
  height: 55px;
  width: 44px;
  display: flex;
  align-items: center;
}
img {
  width: 100%;
}
h4 {
  font-size: 12px;
}
ul {
  width: 100%;
  list-style: none;
  text-transform: uppercase;
  display: flex;
  justify-content: space-around;
}
a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: white;
}
</style>