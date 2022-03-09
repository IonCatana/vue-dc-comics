//HTML 
<template>
  <div id="app">
    <div class="header">
      <div class="img_logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="nav_bar">
        <ul>
          <li v-for="(link, i) in links" :key="i">
            <a :href="link.href" :class=" link.active ? 'active' : ''">{{ link.text }} </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

// JS script Vue
<script>
export default {
  name: "MyHeader",
  data() {
    return {
      links: [
        {
          text: "Characters",
          href: "#",
        },
        {
          text: "Comics",
          href: "#",
          active: true,
        },
        {
          text: "Movies",
          href: "#",
        },
        {
          text: "Tv",
          href: "#",
        },
        {
          text: "Games",
          href: "#",
        },
        {
          text: "Collectibles",
          href: "#",
        },
        {
          text: "Videos",
          href: "#",
        },
        {
          text: "Fans",
          href: "#",
        },
        {
          text: "News",
          href: "#",
        },
        {
          text: "Shop",
          href: "#",
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
}
img {
  width: 100%;
}
.img_logo {
  width: 80px;
  height: 80px;
}
.header {
  padding: 10px 0px 10px 0px;
  width: 70%;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
ul {
  display: contents "";
  list-style: none;
  display: flex;
  text-transform: uppercase;
  font-weight: 700;
  font-size: 14px;
  gap: 20px;
}

a {
  text-decoration: none;
  color: #1c1c1c;
  &:hover {
    color: blue;
    border-bottom: 4px solid blue;
    padding: 0px 0px 38px;
  }
  &:active {
    color: red;
    border-bottom: 4px solid red;
  }
}
</style>