<template>
  <b-container class="last">
    <b-row>
      <b-col cols="12">
        <p class="want">{{ want1 }}</p>
      </b-col>
    </b-row>
    <b-row>
      <b-col cols="12" class="pb-5">
        <p class="text-i">{{ want2 }}</p>
      </b-col>
    </b-row>
    <b-row>
      <b-col cols="12">
        <a class="get" href="">Get It Now</a>
      </b-col>
    </b-row>
  </b-container>
</template>
<script>
export default {
  props: {
    want1: String,
    want2: String,
  },
};
</script>
<style lang="scss" scoped>
.last {
  padding: 0;
}
.want {
  font-size: 30px;
  font-weight: 800;
}
.last {
  padding: 7% 0;
}
.text-i {
  padding: 0 20%;
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