<template>
  <div class="about">
    <b-container>
      <div class="text1">
        <span>{{ text1 }}</span>
      </div>
      <div class="text2">
        <span>{{ text2 }}</span>
      </div>
    </b-container>
  </div>
</template>
<script>
export default {
  props: {
    text1: String,
    text2: String,
  },
};
</script>
<style lang="scss" scoped>
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
</style>