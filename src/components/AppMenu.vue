<template>
  <div class="memnu">
    <b-navbar toggleable="lg" type="dark" variant="dark">
      <b-navbar-brand class="brand" href="#">REEN</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="header">
          <b-nav-item class="a" href="#"
          v-for="(iteam) in iteams" :key="iteam" >{{iteam}}</b-nav-item>
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
            <b-dropdown-item
              v-for="(lang, index) in languages"
              :key="index"
              href="#"
              >{{ lang }}</b-dropdown-item
            >
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
</template>

<script>
export default {
  props: {
    languages: Array,
    iteams: Array
  },
};
</script>

<style lang="scss" scoped>
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
</style>