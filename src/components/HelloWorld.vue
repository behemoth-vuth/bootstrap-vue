<template>
  <div class="bgr">
    <div class="memnu">
      <b-navbar toggleable="lg" type="dark" variant="dark">
        <b-navbar-brand class="brand" href="#">REEN</b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="header">
            <b-nav-item class="a" href="#">Home</b-nav-item>
            <b-nav-item class="a" href="#">Libery</b-nav-item>
            <b-nav-item class="a" href="#">Sing up</b-nav-item>
            <b-nav-item class="a" href="#">Log in</b-nav-item>
            <b-nav-item class="a" href="#">What New</b-nav-item>
            <b-nav-item class="a" href="#">Blog</b-nav-item>
          </b-navbar-nav>

          <b-navbar-nav class="ml-auto">
            <b-nav-form>
              <b-form-input
                size="sm"
                class="mr-sm-2"
                placeholder="Search"
              ></b-form-input>
              <i class="icon-search"></i>
            </b-nav-form>

            <b-nav-item-dropdown text="Lang" right>
              <b-dropdown-item href="#">EN</b-dropdown-item>
              <b-dropdown-item href="#">ES</b-dropdown-item>
              <b-dropdown-item href="#">RU</b-dropdown-item>
              <b-dropdown-item href="#">FA</b-dropdown-item>
            </b-nav-item-dropdown>

            <b-nav-item-dropdown right>
              <template button-content>
                <em>User</em>
              </template>
              <b-dropdown-item href="#">Profile</b-dropdown-item>
              <b-dropdown-item href="#">Sign Out</b-dropdown-item>
            </b-nav-item-dropdown>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>
    <div class="madefordegin">
      <b-container class="h-made">
        <div class="desingers">
          <p>MADE FOR DESINGERS</p>
        </div>
        <div class="made">
          <P
            >The way the Web spread was a piece at a time. So you could take
            html without taking http. So the failure of NEXT was a lesson, don’t
            try to sell it all at one time. Sell each piece on its own merits.
            Never insist that everybody take all. They will take all the pieces
            once they see how it fits together.</P
          >
        </div>
        <div class="get">
          <a href="">Get Started Now</a>
        </div>
      </b-container>
    </div>
    <div class="about">
      <b-container>
        <div class="text1">
          <p>Beautiful.Clean.Reponsive.</p>
        </div>
        <div class="text2">
          <p>
            The way the Web spread was a piece at a time. So you could take html
            without taking http. So the failure of NEXT was a lesson, don’t try
            to sell it all at one time. Sell each piece on its own merits. Never
            insist that everybody take all. They will take all the pieces once
            they see how it fits together.
          </p>
        </div>
      </b-container>
    </div>
    <b-container class="trips">
      <b-row>
        <b-col md="4" sm="12" class="h4 text-left">
          <i class="icon-star"></i>
          Passion
          <p>
            The way the Web spread was a piece at a time. So you could take html
            without taking http. So the failure of NEXT was a lesson, don’t try
            to sell it all at one time. Sell each piece on its own merits. Never
            insist that everybody take all.
          </p>
        </b-col>
        <b-col md="4" sm="12" class="h4 text-left">
          <i class="icon-heart"></i>
          Creativity
          <p>
            The way the Web spread was a piece at a time. So you could take html
            without taking http. So the failure of NEXT was a lesson, don’t try
            to sell it all at one time. Sell each piece on its own merits. Never
            insist that everybody take all.
          </p>
        </b-col>
        <b-col md="4" sm="12" class="h4 text-left">
          <i class="icon-light-bulb"></i>
          Quality
          <p>
            The way the Web spread was a piece at a time. So you could take html
            without taking http. So the failure of NEXT was a lesson, don’t try
            to sell it all at one time. Sell each piece on its own merits. Never
            insist that everybody take all.
          </p>
        </b-col>
      </b-row>
    </b-container>
    <div class="nav">
      <b-container>
        <p class="info1">Check Out Your Lastest Works</p>
        <p class="info2">
          The way the Web spread was a piece at a time. So you could take html
          without taking http
        </p>
      </b-container>
      <b-container>
        <b-row>
          <b-col md="6" sm="12" class="">
            <b-card class="card">
              <img class="card-img-top" :src="image2" alt="" />
              <h6 class="card-title">
                So the failure of NEXT was a lesson, don’t try to sell it all
              </h6>
            </b-card>
          </b-col>
          <b-col md="6" sm="12">
            <b-card class="card">
              <img class="card-img-top" :src="image2" alt="" />
              <h6 class="card-title">
                So the failure of NEXT was a lesson, don’t try to sell it all
              </h6>
            </b-card>
          </b-col>
        </b-row>
      </b-container>
      <b-container>
        <b-row class="image">
          <b-col v-for="i in 4" :key="i" class="img" md="3" cols="6">
            <img :src="images[pageIndex + i - 1]" alt="" />
          </b-col>
          <!-- <b-col class="img" md="3" cols="6"
            ><img :src="image2" alt=""
          /></b-col>
          <b-col class="img" md="3" cols="6"
            ><img :src="image3" alt=""
          /></b-col>
          <b-col class="img" md="3" cols="6"
            ><img :src="image4" alt=""
          /></b-col> -->
        </b-row>
      </b-container>
      <b-container>
        <b-row>
          <b-col>
            <ul class="nav-dots">
              <li class="dot" @click="next(0)"><a></a></li>
              <li class="dot" @click="next(2)"><a></a></li>
              <li class="dot" @click="next(4)"><a></a></li>
            </ul>
          </b-col>
        </b-row>
      </b-container>
    </div>
    <b-container class="last">
      <b-row>
        <b-col col="12">
          <p class="want">Want To Works With Us</p>
        </b-col>
      </b-row>
      <b-row>
        <b-col col="12" class="pb-5">
          <p class="text-i">
            The way the Web spread was a piece at a time. So you could take html
            without taking http. So the failure of NEXT was a lesson, don’t try
            to sell it all at one time.
          </p>
        </b-col>
      </b-row>
      <b-row>
        <b-col col="12">
          <a class="get" href="">Get It Now</a>
        </b-col>
      </b-row>
    </b-container>
    <div class="footer">
      <b-container>
        <b-row class="text-left">
          <b-col md="3" sm="12">
            <p class="row1">Who We Are</p>
            <p class="f-reen">REEN.</p>
            <P
              >The way the Web spread was a piece at a time. So you could take
              html without taking http. So the failure of NEXT was a lesson,
              don’t try to sell it all at one time. Sell each piece on its own
              merits. Never insist that everybody take all. They will take all
              the pieces once they see how it fits together.</P
            >
          </b-col>
          <b-col md="3" sm="12">
            <p class="row1">Lastest Works</p>
            <img :src="image1" alt="" />
          </b-col>
          <b-col md="3" sm="12">
            <p class="row1">Who We Are</p>
            <p class="f-about">
              The way the Web spread was a piece at a time. So you could take
              html without taking http. So the failure of NEXT was a lesson,
              don’t try to sell it all at one time.
            </p>
            <div class="f-icon">
              <i class="icon-facebook"></i>
              <i class="icon-yahoo"></i>
              <i class="icon-instagram"></i>
              <i class="icon-email"></i>
              <i class="icon-twitter-alt"></i>
            </div>
            <P>The way the Web spread was a piece at a time.</P>
          </b-col>
          <b-col md="3" sm="12">
            <p class="row1">Get In Touch</p>
            <P
              >The way the Web spread was a piece at a time. So you could take
              html without taking http.</P
            >
            <div class="f-seach">
              <input class="text-seach" type="text" value="" />
              <a class="get" href="">Get It Now</a>
            </div>
          </b-col>
        </b-row>
      </b-container>
    </div>
  </div>
</template>
<script>
import image1 from "../assets/styles/a.jpeg";
import image2 from "../assets/styles/b.jpeg";
import image3 from "../assets/styles/c.jpeg";
import image4 from "../assets/styles/d.jpg";
import image5 from "../assets/styles/e.jpg";
import image6 from "../assets/styles/g.jpg";
export default {
  data() {
    return {
      image1,
      image2,
      image3, image4, image5, image6,
      images: [image1, image2, image3, image4, image5, image6, image2, image1],
      pageIndex: 0,
    };
  },

  methods: {
    next(from) {
      this.pageIndex = from;
      if (this.pageIndex >= this.images.length) {
        this.pageIndex = 0;
      }
    },
  },
};
</script>


<style lang="scss">
.nav-dots {
  z-index: 1;
  display: flex;
  list-style-type: none;
  margin-top: 40px;
  justify-content: center;
  padding: 0;

  .dot {
    width: 1em;
    height: 1em;
    margin: 1em;

    a {
      position: relative;
      display: block;
      height: 1em;
      line-height: 1em;

      &::before {
        position: absolute;
        content: "";
        width: 100%;
        height: 100%;
        background: white;
        border-radius: 50%;
      }

      &:hover::before {
        background: black;
      }

      &.active::before {
        background: rgba(255, 255, 255, 0.8);
      }
    }
  }
}
.memnu {
  position: fixed;
  z-index: 1;
  width: 100%;
}
.header {
  margin: auto;
}
.brand {
  font-size: larger;
  font-weight: 900;
}
.a {
  padding: 0 10px;
  font-weight: 900;
}
#nav-collapse {
  text-align: center;
}
.text-seach {
  opacity: 0.5;
  width: 90%;
  margin-right: 10px;
  margin-top: 3px;
}
.madefordegin {
  position: relative;
  background-image: url("data:image/jpeg;base64,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");
  background-size: cover;
  background-repeat: no-repeat;
  height: 600px;
}
.h-made {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
.desingers {
  font-weight: 900;
  color: white;
  font-size: 40px;
}
.made {
  color: white;
}
.get {
  display: inline-block;
  padding: 10px 16px;
  color: white;
  background-color: rgb(21, 72, 78);
}
.get:hover {
  opacity: 0.5;
}
.get a {
  color: white;
}
.about {
  padding: 5% 0;
}
.text1 {
  font-size: 25px;
  font-weight: 800;
  padding-bottom: 2%;
}
.text2 {
  padding: 0 10%;
}
.card-title {
  padding-top: 20px;
}
.trips i {
  font-size: xx-large;
  color: rgb(2, 123, 136);
  font-weight: 900;
}
.trips p {
  font-size: 1rem;
  font-weight: 400;
  padding-left: 38px;
  padding-bottom: 20%;
}
.nav {
  background-color: silver;
  padding: 7% 0;
}
.info1 {
  font-size: 30px;
  font-weight: 800;
}
.image {
  padding-top: 30px;
}
.image img {
  width: 100%;
  height: 200px;
  padding-bottom: 30px;
}
.want {
  font-size: 30px;
  font-weight: 800;
}
.text-i {
  padding: 0 20%;
}
.last {
  padding: 7% 0;
}
.row1 {
  font-size: 20px;
  font-weight: 700;
}
.footer {
  padding: 5% 0;
  background-color: rgb(22, 37, 58);
  color: white;
}
.f-reen {
  font-size: 35px;
  font-weight: 800;
}
.f-imgae {
  font-weight: 20px;
}
.f-icon i {
  padding: 0 10px;
  font-size: 20px;
}
.f-icon i:hover {
  opacity: 0.5;
  cursor: pointer;
}
.f-seach .text-seach {
  width: 50%;
  padding: 8px 0;
  margin: 0;
}
.f-seach a {
  width: 50%;
  margin: 0;
}
.footer img {
  font-size: 20px;
  height: 135px;
}

.card-body {
  padding: 0 !important;
}
</style>