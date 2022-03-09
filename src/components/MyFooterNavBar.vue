<template>
  <div id="app">
    <div class="footer_navbar">
      <div class="main_navbar">
        <div class="sign_up">
          <button>SIGN-UP NOW!</button>
        </div>
        <div class="follow_us">
          <ul>
            <h2>{{ titolo }}</h2>
            <li v-for="(link, i) in FollowUs" :key="i">
              <a :href="link.href"
                ><img :src="require('../assets/img/' + link.imgUrl)"/></a>
            </li>            
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyFooterNavBar",
  data() {
    return {
      titolo: "Follow Us",
      FollowUs: [
        {
          href: "#",
          imgUrl: "footer-facebook.png",
        },
        {
          href: "#",
          imgUrl: "footer-twitter.png",
        },
        {
          href: "#",
          imgUrl: "footer-youtube.png",
        },
        {
          href: "#",
          imgUrl: "footer-pinterest.png",
        },
        {
          href: "#",
          imgUrl: "footer-periscope.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.footer_navbar {
  width: 100vw;
  background-color: #303030;
  height: 100px;
}
.main_navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 100%;
  width: 70%;
  margin: 0 auto;
}
button {
  padding: 15px 20px;
  border: 1px solid #0282f9;
  background-color: #303030;
  color: white;
}

ul {
  display: flex;
  align-items: center;
  list-style: none;
  gap: 20px;
}
h2 {
  text-transform: uppercase;
  color: #0282f9;
  padding-right: 10px;
}
a {
  text-decoration: none;
}
</style>