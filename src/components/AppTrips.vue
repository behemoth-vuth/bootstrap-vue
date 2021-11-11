<template>
  <b-container class="trips">
    <b-row>
      <b-col md="4" sm="12" class="h4 text-left">
        <i class="icon-star"></i>
        Passion
        <p>{{ trip1 }}</p>
      </b-col>
      <b-col md="4" sm="12" class="h4 text-left">
        <i class="icon-heart"></i>
        Creativity
        <p>{{ trip2 }}</p>
      </b-col>
      <b-col md="4" sm="12" class="h4 text-left">
        <i class="icon-light-bulb"></i>
        Quality
        <p>{{ trip3 }}</p>
      </b-col>
    </b-row>
  </b-container>
</template>
<script>
export default {
  props: {
    trip1: String,
    trip2: String,
    trip3: String,
  },
};
</script>
<style lang="scss" scoped>
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
</style>