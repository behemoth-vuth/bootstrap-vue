<template>
  <div class="nav">
    <b-container>
      <p class="info1">{{ info1 }}</p>
      <p class="info2">{{ info2 }}</p>
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
      pageIndex: 0,
      images: [image1, image2, image3, image4, image5, image6, image2, image1],
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

  props: {
    image2: String,
    info1: String,
    info2: String,
  },
};
</script>
<style lang="scss" scoped>
.nav {
  background-color: silver;
  padding: 7% 0;
}
.info1 {
  font-size: 30px;
  font-weight: 800;
}
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
.card-title {
  padding-top: 20px;
}
.card-body {
  padding: 0 !important;
}
.image {
  padding-top: 30px;
}
.image img {
  width: 100%;
  height: 200px;
  padding-bottom: 30px;
}
</style>