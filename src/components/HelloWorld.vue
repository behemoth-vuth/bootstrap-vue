<template>
  <div class="bgr">
    <app-menu :languages="languages" :iteams="iteams"></app-menu>
    <app-made :title="title" :get="get" :sub="sub"></app-made>
    <app-about :text1="text1" :text2="text2"></app-about>
    <app-trips :trip1="trip1" :trip2="trip2" :trip3="trip3"></app-trips>
    <app-navi :info1="info1" :info2="info2" :image2="image2"></app-navi>
    <app-last :want1="want1" :want2="want2"></app-last>
    <app-bottom
      :who="who"
      :about1="about1"
      :about2="about2"
      :about3="about3"
      :about4="about4"
      :image1="image1"
    ></app-bottom>
  </div>
</template>
<script>
import image1 from "../assets/styles/a.jpeg";
import image2 from "../assets/styles/b.jpeg";
import image3 from "../assets/styles/c.jpeg";
import image4 from "../assets/styles/d.jpg";
import image5 from "../assets/styles/e.jpg";
import image6 from "../assets/styles/g.jpg";
import AppMenu from "./AppMenu.vue";
import AppMade from "@/components/AppMade.vue";
import AppAbout from "./AppAbout.vue";
import AppTrips from "@/components/AppTrips.vue";
import AppNavi from "./AppNavi.vue";
import AppLast from "./AppLast.vue";
import AppBottom from "./AppBottom.vue";

export default {
  components: {
    AppMenu,
    AppMade,
    AppAbout,
    AppTrips,
    AppNavi,
    AppLast,
    AppBottom,
  },
  data() {
    return {
      image1,
      image2,
      image3,
      image4,
      image5,
      image6,
      languages: ["EN", "VI", "JA"],
      iteams: ["Home", "Libery", "Sing up", "Log in", "What New"],
      title: "Made For Desginer",
      get: "Get Started Now",
      sub: "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time. Sell each piece on its own merits. Never insist that everybody take all. They will take all the pieces once they see how it fits together.",
      text1: "Beautiful.Clean.Reponsive.",
      text2:
        "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time. Sell each piece on its own merits. Never insist that everybody take all. They will take all the pieces once they see how it fits together.",
      trip1:
        "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time. Sell each piece on its own merits. Never insist that everybody take all.",
      trip2:
        "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time. Sell each piece on its own merits. Never insist that everybody take all.",
      trip3:
        "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time. Sell each piece on its own merits. Never insist that everybody take all.",
      info1: "Check Out Your Lastest Works",
      info2:
        "The way the Web spread was a piece at a time. So you could take html without taking http",
      want1: "Want To Works With Us",
      want2:
        "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time.",
      who: "Who We Are",
      about1:
        "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time. Sell each piece on its own merits. Never insist that everybody take all. They will take all the pieces once they see how it fits together.",
      about2:
        "The way the Web spread was a piece at a time. So you could take html without taking http. So the failure of NEXT was a lesson, don’t try to sell it all at one time.",
      about3: "The way the Web spread was a piece at a time.",
      about4:
        "The way the Web spread was a piece at a time. So you could take html without taking http.",
    };
  },
};
</script>

<style lang="scss" scoped>
</style>