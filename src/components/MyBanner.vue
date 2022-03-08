<template>
  <div id="app">
    <div class="banner_blu">
      <div class="banner_items">
        <ul>
          <li>
            <a href="#">
              <div class="img_banner">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
              </div>
              <h4>Digital Comics</h4>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="img_banner">
                <img src="../assets/img/buy-comics-merchandise.png" alt="" />
              </div>
              <h4>Dc Merchandise</h4>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="img_banner">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
              </div>
              <h4>Subscriptions</h4>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="img_banner">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
              </div>
              <h4>Comic Shop Locator</h4>
            </a>
          </li>
          <li>
            <a href="#">
              <div class="img_banner">
                <img src="../assets/img/buy-dc-power-visa.png" alt="" />
              </div>
              <h4>Dc Power Visa</h4>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

// JS script Vue
<script>
export default {};
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
  width: 43px;
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
  justify-content: space-between;
}
a {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: white;
}
</style>