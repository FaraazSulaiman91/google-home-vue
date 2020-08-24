<template>
  <div class="bottom-bar">
    <b-navbar class="bottom-nav" fixed="bottom">
      <b-navbar-nav>
        <b-nav-item>Advertising</b-nav-item>
        <b-nav-item>Business</b-nav-item>
        <b-nav-item>About</b-nav-item>
        <b-nav-item>How Search Works</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item>Privacy</b-nav-item>
        <b-nav-item>Terms</b-nav-item>
        <b-nav-item>Settings</b-nav-item>
      </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'BottomBar',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bottom-nav {
  background: #f2f2f2;
  border-top: 1px solid #e4e4e4;
}
</style>
