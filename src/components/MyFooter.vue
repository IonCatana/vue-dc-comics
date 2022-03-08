//HTML 
<template>
  <div id="app">
    <div class="bg_dc">
      <div class="footer_contain">
        <div class="side_left">
          <div class="container_comics_shop">
            <ul>
              <h3>{{ titolo1 }}</h3>
              <li v-for="(link, i) in DcComics" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
            <ul class="container_shop">
              <h3>{{ titolo2 }}</h3>
              <li v-for="(link, i) in Shop" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="container_dc">
            <ul>
              <h3>{{ titolo3 }}</h3>
              <li v-for="(link, i) in DC" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
          </div>
          <div class="container_sites">
            <ul>
              <h3>{{ titolo4 }}</h3>
              <li v-for="(link, i) in Sites" :key="i">
                <a :href="link.href">{{ link.text }}</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="side_right"></div>
      </div>
    </div>
  </div>
</template>

// JS script Vue
<script>
export default {
  name: "MyFooter",
  data() {
    return {
      titolo1: "Dc Comics",
      titolo2: "Shop",
      titolo3: "DC",
      titolo4: "Sites",
      DcComics: [
        {
          href: "#",
          text: "Characters",
        },
        {
          href: "#",
          text: "Comics",
        },
        {
          href: "#",
          text: "Movies",
        },
        {
          href: "#",
          text: "TV",
        },
        {
          href: "#",
          text: "Games",
        },
        {
          href: "#",
          text: "Videos",
        },
        {
          href: "#",
          text: "News",
        },
      ],
      Shop: [
        {
          href: "#",
          text: "Shop DC",
        },
        {
          href: "#",
          text: "Shop DC Collectibles",
        },
      ],
      DC: [
        {
          href: "#",
          text: "Terms Of Use",
        },
        {
          href: "#",
          text: "Privacy policy (New)",
        },
        {
          href: "#",
          text: "Ad Choices",
        },
        {
          href: "#",
          text: "Adverstising",
        },
        {
          href: "#",
          text: "Jobs",
        },
        {
          href: "#",
          text: "Subscriptions",
        },
        {
          href: "#",
          text: "Talent Workshops",
        },
        {
          href: "#",
          text: "CPSC Certificates",
        },
        {
          href: "#",
          text: "Ratings",
        },
        {
          href: "#",
          text: "Shop Help",
        },
        {
          href: "#",
          text: "Contact Us",
        },
      ],
      Sites: [
        {
          href: "#",
          text: "DC",
        },
        {
          href: "#",
          text: "MAD Magazine",
        },
        {
          href: "#",
          text: "DC Kids",
        },
        {
          href: "#",
          text: "DC universe",
        },
        {
          href: "#",
          text: "DC Power Visa",
        },
      ],
    };
  },
};
</script>

// Style CSS
<style lang="scss" scoped>
h3 {
  padding: 0px 0px 15px;
  color: white;
  text-transform: uppercase;
}
.bg_dc {
  height: 380px;
  width: 100vw;
  background-image: url(../assets/img/footer-bg.jpg);
}
.footer_contain {
  display: flex;
  height: 380px;
  width: 70%;
  margin: 0 auto;
}
.container_shop {
  padding-top: 15px;
}
.side_left {
  width: 50%;
  display: flex;
  gap: 30px;
  padding: 40px 0px;
}
.side_right {
  background-image: url(../assets/img/dc-logo-bg.png);
  object-fit: contain;
  background-repeat: no-repeat;
  background-position: center;
  width: 50%;
}
ul {
  display: contents "";
  list-style: none;
  font-weight: 700;
  font-size: 14px;
  gap: 20px;
}

a {
  font-size: 11px;
  line-height: 20px;
  text-decoration: none;
  color: grey;
  &:hover {
    color: blue;
  }
}
</style>