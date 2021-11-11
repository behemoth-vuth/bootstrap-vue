<template>
  <div class="footer">
    <b-container>
      <b-row class="text-left">
        <b-col md="3" sm="12">
          <p class="row1">{{ who }}</p>
          <p class="f-reen">REEN.</p>
          <p>{{ about1 }}</p>
        </b-col>
        <b-col md="3" sm="12">
          <p class="row1">Lastest Works</p>
          <img :src="image1" alt="" />
        </b-col>
        <b-col md="3" sm="12">
          <p class="row1">{{ who }}</p>
          <p class="f-about">{{ about2 }}</p>
          <div class="f-icon">
            <i class="icon-facebook"></i>
            <i class="icon-yahoo"></i>
            <i class="icon-instagram"></i>
            <i class="icon-email"></i>
            <i class="icon-twitter-alt"></i>
          </div>
          <p>{{ about3 }}</p>
        </b-col>
        <b-col md="3" sm="12">
          <p class="row1">Get In Touch</p>
          <p>{{ about4 }}</p>
          <div class="f-seach">
            <input class="text-seach" type="text" value="" />
            <a class="get" href="">Get It Now</a>
          </div>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<script>
export default {
  props: {
    who: String,
    about1: String,
    about2: String,
    about3: String,
    about4: String,
    image1: String,
  },
};
</script>
<style lang="scss" scoped>
.text-seach {
  opacity: 0.5;
  width: 90%;
  margin-right: 10px;
  margin-top: 3px;
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
.row1 {
  font-size: 20px;
  font-weight: 700;
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
</style>