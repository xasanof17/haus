<template>
  <div id="app">
    <div class="header__top" v-show="close">
      <div class="container">
        <div class="header__top-content">
          <p class="header__top-text">Free shipping on orders over $50</p>
          <button class="header__top-close" v-on:click="topMenu()"><svg width="12" height="12" viewBox="0 0 12 12"
              fill="none" xmlns="http://www.w3.org/2000/svg">
              <path fill-rule="evenodd" clip-rule="evenodd"
                d="M9.8995 0L11.3137 1.41421L7.071 5.657L11.3137 9.8995L9.8995 11.3137L5.657 7.071L1.41421 11.3137L0 9.8995L4.243 5.657L0 1.41421L1.41421 0L5.657 4.243L9.8995 0Z"
                fill="black" />
            </svg>
          </button>
        </div>
      </div>
    </div>

    <header class="header">
      <div class="header__left">
        <img src="../assets/img/header.svg" class="header__img" alt="">
      </div>
      <nav class="header__nav" v-bind:style="{ 'background': black ? 'black' : '' }">
        <div class=" container">
          <div class="header__nav-content">
            <ul class="header__nav-content_list">
              <li class="header__nav-content_list-item"><a href="#!" class="header__nav-content_list-item_link">shop</a>
              </li>
              <li class="header__nav-content_list-item"><a href="#!"
                  class="header__nav-content_list-item_link">membership</a></li>
              <li class="header__nav-content_list-item"><a href="#!" class="header__nav-content_list-item_link">our
                  story</a></li>
            </ul>
            <a href="#!" class="logo"><img src="../assets/img/logo.svg" alt=""></a>
            <ul class="header__nav-content_list">
              <li class="header__nav-content_list-item"><a href="#!"
                  class="header__nav-content_list-item_link">Newsletter</a></li>
              <li class="header__nav-content_list-item"><a href="#!"
                  class="header__nav-content_list-item_link">Account</a></li>
              <li class="header__nav-content_list-item"><a href="#!" class="header__nav-content_list-item_link">Cart
                  (<span>0</span>)</a></li>
            </ul>
            <div class="header__nav-smallscreen">
              <div class="menu-btn" v-on:click="menu()">
                <span class="bar"></span>
                <span class="bar"></span>
                <span class="bar"></span>
              </div>
              <Transition name="op">
                <div class="header__nav-smallscreen_overlay" ref="back" v-show="show">
                  <div class="menu-btn active" v-on:click="menu()">
                    <span class="bar"></span>
                    <span class="bar"></span>
                    <span class="bar"></span>
                  </div>
                  <ul class="header__nav-smallscreen_overlay-list">
                    <li class="header__nav-smallscreen_overlay-item">
                      <a href="/">shop</a>
                    </li>
                    <li class="header__nav-smallscreen_overlay-item">
                      <a href="/">membership</a>
                    </li>
                    <li class="header__nav-smallscreen_overlay-item">
                      <a href="/">our
                        story</a>
                    </li>
                    <li class="header__nav-smallscreen_overlay-item">
                      <a href="/">Newsletter</a>
                    </li>
                    <li class="header__nav-smallscreen_overlay-item">
                      <a href="/">Account</a>
                    </li>
                  </ul>
                </div>
              </Transition>

            </div>
          </div>
        </div>
      </nav>
      <div class="header__right">
        <div class="header__right-box">
          <h1 class="header__right-box-title">Alcohol for the modern drinker</h1>
          <p class="header__right-box-text">Light and refreshing flavors made with real, clean ingredients you can feel
            good
            about. Just pour, sip, and enjoy.
          </p>
          <div class="header__right-box-button">
            <button class="header__right-box-button-btn all-btn">Shop All</button>
          </div>
        </div>
      </div>
    </header>
    <main>
      <section class="logos">
        <div class="container">
          <div class="logos__content">
            <div class="row logo__row">
              <div class="col-12 col-lg-4 col-md-6 col-sm-6 logo__box">
                <p class="logos__txt">"What makes Haus so special is its incredible flavors."</p>
                <img src="../assets/img/logo1.svg" alt="">
              </div>
              <div class="col-12 col-lg-4 col-md-6 col-sm-6 logo__box">
                <p class="logos__txt">"What makes Haus so special is its incredible flavors."</p>
                <img src="../assets/img/logo2.svg" alt="">
              </div>
              <div class="col-12 col-lg-4 col-md-6 col-sm-6 logo__box">
                <p class="logos__txt">"What makes Haus so special is its incredible flavors."</p>
                <img src="../assets/img/logo3.svg" alt="">
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="natural">
        <div class="container">
          <div class="natural__content">
            <div class="natural__top">
              <h2 class="natural__title">Made with natural ingredients, nothing fake</h2>
              <span class="natural__span">Shop All Flavors</span>
            </div>
            <div class="row natural__boxs">
              <div class="col-12 col-lg-4 col-md-4 natural__box">
                <div class="natural__box-head">
                  <img src="../assets/img/card1.png" alt="vino">
                </div>
                <div class="natural__box-body">
                  <h3>The Sampler Kit</h3>
                  <p>Try a variety of Haus flavors with our customizable four-bottle kit. Each bottle serves 2-3 drinks.
                  </p>
                  <div class="natural__button">
                    <button class="natural__btn all-btn">Shop Now</button>
                  </div>
                </div>
              </div>
              <div class="col-12 col-lg-4 col-md-4 natural__box">
                <div class="natural__box-head">
                  <img src="../assets/img/card2.png" alt="vino">
                </div>
                <div class="natural__box-body">
                  <h3>Grapefruit Jalapeño</h3>
                  <p>Light and refreshing, this aperitif is a bright blend of citrus with a subtle kick of fresh
                    jalapeño.
                  </p>
                  <div class="natural__button">
                    <button class="natural__btn all-btn">Shop Now</button>
                  </div>
                </div>
              </div>
              <div class="col-12 col-lg-4 col-md-4 natural__box">
                <div class="natural__box-head">
                  <img src="../assets/img/card3.png" alt="vino">
                </div>
                <div class="natural__box-body">
                  <h3>Citrus Flower </h3>
                  <p>A fresh Californian take on the apéritif. Made with crisp lemon and subtle elderflower.
                  </p>
                  <div class="natural__button">
                    <button class="natural__btn all-btn">Shop Now</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="intro">
        <div class="container">
          <div class="intro__content">
            <div class="intro__top">
              <img src="../assets/img/section.png" alt="">
            </div>
            <div class="intro__bottom">
              <div class="row">
                <div class="col-12 col-lg-6 col-md-6 col-sm-6">
                  <h2>An intro to apéritifs</h2>
                </div>
                <div class="col-12 col-lg-6 col-md-6 col-sm-6">
                  <p>Apéritifs are a category of spirits with complex flavors derived from fruits, herbs, and
                    botanicals. Their lighter alcohol content (less than whiskey, more than wine) makes them perfect to
                    sip all evening.</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="drink">
        <div class="container">
          <div class="drink__content">
            <div class="row">
              <div class="col-12 col-lg-4">
                <div class="col drink__box">
                  <h3>Easy to drink</h3>
                  <p>The perfect anytime drink, sip Haus on its own or with simple mixers you probably already have like
                    soda or tonic.</p>
                </div>
                <div class="col drink__box">
                  <h3>Natural ingredients. Nothing fake.</h3>
                  <p>Artificial ingredients and refined sugars are a big culprit in hangovers. Feel good about what’s in
                    your glass that night — and the next day.</p>
                </div>
                <div class="col drink__box">
                  <h3>Delivered to your door</h3>
                  <p>We blend, bottle, and ship our products straight from Sonoma, CA to your doorstep.</p>
                </div>
              </div>
              <div class="col-12 col-lg-8 drink__img">
                <img src="../assets/img/section2.png" alt="">
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="blackblock">
        <div class="container">
          <div class="blackblock__content">
            <div class="row">
              <div class="col-12 col-lg-4 col-md-4 blackblock__box">
                <p>“Haus has found the solution I didn’t really know I was looking for!”</p>
                <span class="auhtor">— Susan</span>
                <span class="verified">verified buyer</span>
              </div>
              <div class="col-12 col-lg-4 col-md-4 blackblock__box">
                <p>“Haus has found the solution I didn’t really know I was looking for!”</p>
                <span class="auhtor">— Susan</span>
                <span class="verified">verified buyer</span>
              </div>
              <div class="col-12 col-lg-4 col-md-4 blackblock__box">
                <p>“Haus has found the solution I didn’t really know I was looking for!”</p>
                <span class="auhtor">— Susan</span>
                <span class="verified">verified buyer</span>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="producer">
        <div class="container">
          <div class="producer__content">
            <div class="row">
              <div class="col-12 col-lg-6 col-md-6 col-sm-6 producer__box"><img src="../assets/img/section3.png" alt="">
              </div>
              <div class="col-12 col-lg-6 col-md-6 col-sm-6 producer__box">
                <h2>We do things differently than most producers</h2>
                <p>Our flavors are derived from real fruits, herbs, and botanicals, not ingredients from a lab. We leave
                  out the artificial ingredients and excess sugar, and tell you what’s inside. It’s a better way to
                  drink.</p>
                <a href="#!">LEARN MORE</a>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section class="mood">
        <div class="container">
          <div class="mood__content">
            <div class="row">
              <div class="col-12 col-lg-6 col-md-6 mood__box">
                <div class="mood__top">
                <h3>Set the mood</h3>
                <p>Curated playlists from Woody + Helena, plus some of our friends and favorite brands.</p>
                <button class="all-btn">Spotify</button>
                </div>
                <div class="mood__bottom"></div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>
    <footer class="footer">
    <div class="container">
    <p>This Website created by Javohir</p>
    </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      show: false,
      close: true,
      black: false,
    }
  },
  methods: {
    menu() {
      this.show = !this.show
    },
    topMenu() {
      this.close = false
    },
    scrollMenu() {
      if (window.scrollY > 48) {
        this.black = true
      } else if (window.scrollY < 48) {
        this.black = false
      }
    },

  },
  mounted() {
    window.addEventListener("scroll", this.scrollMenu)
  },

}
</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700;900&display=swap');

:root {
  --white: #fff;
  --dark: #191919;
  --black: #000;
  --darkPink: #996B60;
  --body: #E5E5E5;
  --lightWhite: rgba(255, 255, 255, 0.6);
  --gray: #818181;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  list-style: none;
  text-decoration: none;
  outline: none;
  border: none;
}

.all-btn {
  width: 180px;
  height: 52px;
  font-weight: 400;
  font-size: 15px;
  line-height: 14px;
  letter-spacing: 1px;
  text-transform: uppercase;
}

body {
  margin: 0;
  font-family: 'Roboto';
  /* scroll-behavior: smooth;*/
}

.container {
  max-width: 1320px;
  width: 100%;
  margin: 0 auto;
  padding: 0 12px;
}

ul {
  margin-bottom: 0;
  padding-left: 0;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'LiberationSerif';
}

.header__top {
  position: relative;
  z-index: 10;
  padding: 15px 0;
  background: var(--dark);
}

.header__top .container {
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

.header__top .header__top-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 58%;
}

.header__top-text {
  font-weight: 400;
  font-size: 14px;
  line-height: 18px;
  text-align: center;
  color: var(--white);
  margin-bottom: 0;
}

.header__top-close {
  font-size: 15px;
  color: var(--white);
  display: flex;
  align-items: center;
  justify-content: center;
  background: transparent;
  border: none;
  cursor: pointer;
}

.header__top-close svg path {
  fill: #fff;
}

.header {
  position: relative;
  height: 100vh;
  background: var(--darkPink);
}

.header__left {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 50%;
}

.header__left img {
  width: 100%;
  height: 100%;
  user-select: none;
}

.header__right {
  position: absolute;
  top: 0;
  right: 0;
  width: 50%;
  height: 100%;
  display: flex;
  align-items: stretch;
  justify-content: flex-start;
  padding: 0 0 100px 60px;
}

.header__right-box {
  display: flex;
  align-items: flex-start;
  justify-content: center;
  flex-direction: column;
}

.header__right-box-title {
  font-weight: 400;
  font-size: 73px;
  line-height: 96px;
  color: var(--white);
  max-width: 457px;
  width: 100%;
  margin-bottom: 35px;
}

.header__right-box-text {
  font-weight: 400;
  font-size: 18px;
  line-height: 32px;
  color: var(--white);
  max-width: 572px;
  width: 100%;
  margin-bottom: 50px;
}

.header__right-box-button {
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

.header__right-box-button-btn {
  background: transparent;
  border: 1px solid var(--white);
  position: relative;
  z-index: 2;
  transition: .5s ease;
}

.header__right-box-button-btn::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 0;
  height: 100%;
  background: var(--black);
  transition: .5s ease;
  z-index: -1;
}

.header__right-box-button-btn:hover {
  color: var(--white);
}

.header__right-box-button-btn:hover::after {
  width: 100%;
}

.header__nav {
  position: sticky;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 5;
  padding: 25px 0;
}

.header__nav-content {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.header__nav-content_list {
  display: flex;
}

.header__nav-content_list-item {
  margin: 0 30px;
}

.header__nav-content_list-item_link {
  font-weight: 400;
  font-size: 14px;
  line-height: 18px;
  color: var(--white);
  text-decoration: none;
  text-transform: uppercase;
  transition: .5s ease;
}

.header__nav-content_list-item_link:hover {
  color: inherit;
}

.header__nav-smallscreen {
  left: -100%;
}

.menu-btn {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  align-content: space-between;
  cursor: pointer;
  transition: .5s ease;
  position: relative;
}

.menu-btn.active .bar:nth-of-type(1) {
  transform: rotate(45deg);
  position: absolute;
  bottom: 0;
  right: 0px;
  background: var(--white);
}

.menu-btn.active .bar:nth-of-type(2) {
  width: 0;
}

.menu-btn.active .bar:nth-of-type(3) {
  transform: rotate(-45deg);
  position: absolute;
  top: 0;
  right: 0px;
  background: var(--white);
}

.header__nav-smallscreen_overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  background: rgba(0, 0, 0, 0.9);
  padding-top: 10%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.header__nav-smallscreen_overlay .menu-btn {
  position: absolute;
  top: 30px;
  right: 10px;
  background: var(--black);
}

.header__nav-smallscreen_overlay-list {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.header__nav-smallscreen_overlay-item {
  margin: 10px 0;
}

.header__nav-smallscreen_overlay-item a {
  text-decoration: none;
  color: var(--white);
  font-size: 22px;
  text-transform: uppercase;
}

.bar {
  height: 2px;
  width: 30px;
  background: var(--white);
  margin-bottom: 8px;
}

.bar:last-child {
  margin-bottom: 0;
}

.logos {
  margin-top: 55px;
  margin-bottom: 50px;
}

.logos__content {
  padding-bottom: 40px;
  border-bottom: 1px solid #BDBDBD;
}

.logo__box {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.logos__txt {
  font-weight: 400;
  font-size: 18px;
  line-height: 32px;
  max-width: 290px;
  width: 100%;
  text-align: center;
}

.natural {
  margin-top: 100px;
}

.natural__content {
  padding-bottom: 140px;
  border-bottom: 1px solid #BDBDBD;
}

.natural__top {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  margin-bottom: 120px;
}

.natural__title {
  font-weight: 400;
  font-size: 64px;
  line-height: 80px;
  text-align: center;
  max-width: 673px;
  width: 100%;
  margin-bottom: 25px;
}

.natural__span {
  font-weight: 400;
  font-size: 12px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: var(--black);
}

.natural__box {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.natural__box-head {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.natural__box-head img {
  max-width: 100%;
  width: 100%;
  height: 438px;
}

.natural__box-body {
  padding-top: 55px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}

.natural__box-body h3 {
  font-weight: 400;
  font-size: 30px;
  line-height: 44px;
  color: var(--black);
}

.natural__box-body p {
  font-weight: 400;
  font-size: 16px;
  line-height: 28px;
  text-align: center;
  color: var(--black);
}

.natural__btn {
  background: var(--dark);
  color: var(--white);
}

.intro {
  margin-top: 60px;
}

.intro__top {
  width: 100%;
}

.intro__top img {
  width: 100%;
}

.intro__bottom {
  margin-top: 55px;
  padding-bottom: 95px;
  border-bottom: 1px solid #BDBDBD;
}

.drink {
  margin-top: 60px;
}

.drink__box h3 {
  font-weight: 400;
  font-size: 30px;
  line-height: 44px;
  color: var(--black);
  margin-bottom: 18px;
}

.drink__box p {
  font-weight: 400;
  font-size: 18px;
  line-height: 32px;
  color: var(--black);
  max-width: 373px;
  width: 100%;
}

.drink__img img {
  width: 100%;
}

.blackblock {
  margin: 55px 0;
  background: var(--black);
}

.blackblock__content {
  padding: 55px 0;
}

.blackblock__box {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  color: var(--white);
}

.blackblock__box p {
  font-weight: 400;
  font-size: 18px;
  line-height: 32px;
  text-align: center;
  max-width: 300px;
  width: 100%;
}

.blackblock__box span {
  margin: 7px 0;
}

.blackblock__box .auhtor {
  font-weight: 400;
  font-size: 14px;
  line-height: 21px;
  text-align: center;
}

.blackblock__box .verified {
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  text-align: center;
  color: var(--gray);
}

.producer__content {
  padding: 60px 0;
}

.producer__box img {
  width: 80%;
}

.mood {
  padding: 60px 0;
  margin-top: 60px;
  background: url('../assets/img/main.png') no-repeat center / cover;
  min-height: 568px;
}


.mood__top {
  padding: 40px 70px;
  background: var(--black);
  color: var(--white);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.mood__top h3{
  font-weight: 400;
font-size: 55px;
line-height: 80px;
}
.mood__top p{
font-weight: 400;
font-size: 16px;
line-height: 28px;
text-align: center;
}

@media (max-width: 1440px) {
  .header__right-box {
    justify-content: flex-end;
  }
}

@media (max-width: 1024px) {
  .header__left {
    top: 0;
  }

  .header__nav {
    padding: 10px 0;
  }

  .header__right {
    padding: 0 0 130px 40px;
  }

  .header__right-box-title {
    font-size: 65px;
    line-height: 85px;
  }
}
.footer{
  padding: 20px 0;
}
.footer .container{
  display: flex;
  align-items: center;
  justify-content: center;
}
.footer p {
  color: var(--dark);
  font-size: 20px;
  line-height: 25px;
  margin-bottom: 0;
}

@media (max-width: 768px) {
  .header__top .header__top-content {
    width: 62%;
  }

  .header__nav {
    padding: 13px 0;
  }

  .header__nav-content_list {
    display: none;
  }

  .header__nav-smallscreen {
    display: flex;
  }

  .header__right {
    padding: 0 0 150px 30px;
  }

  .logo__row {
    justify-content: center;
  }

  .logo__box {
    margin: 20px 0;
  }
}

@media (max-width: 500px) {
  .header__top .header__top-content {
    width: 70%;
  }

  .header__left {
    display: none;
  }

  .header__right {
    top: 5%;
    left: 0;
    width: 100%;
    padding: 0 0 148px 15px;
  }

  .header__right-box-title {
    font-size: 52px;
    line-height: 80px;
  }

  .natural__title {
    font-size: 45px;
    line-height: 70px;
  }

  .natural__box {
    margin: 20px 0;
  }

  .natural__content {
    padding-bottom: 60px;
    border-bottom: 1px solid #BDBDBD;
  }

  .blackblock__box {
    margin: 20px 0;
  }
  .mood__top{
        padding: 29px 30px;
  }
}

@media (max-width: 425px) {
  .header__top .header__top-content {
    width: 75%;
  }
}

@media (max-width: 375px) {
  .header__top .header__top-content {
    width: 80%;
  }
}

@media (max-width: 320px) {
  .header__top .header__top-content {
    width: 90%;
  }
}

.op-enter-active,
.op-leave-active {
  transition: opacity 0.5s ease;
}

.op-enter-from,
.op-leave-to {
  left: 0;
}

.op-enter-active,
.op-leave-active {
  transition: 0.5s;
}

.op-enter-from,
.op-leave-to {
  left: -100%
}
</style>
