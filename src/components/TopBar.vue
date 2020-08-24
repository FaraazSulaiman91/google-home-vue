<template>
  <div class="top-bar">
    <b-navbar>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-navbar-nav>
            <b-nav-item href="https://mail.google.com/mail/?tab=wm&authuser=0&ogbl">Gmail</b-nav-item>
            <b-nav-item href="https://www.google.co.za/imghp?hl=en&tab=wi&authuser=0&ogbl">Images</b-nav-item>
          </b-navbar-nav>

          <b-nav-item-dropdown html="" right no-caret>
            <template v-slot:button-content>
              <BIconGrid3x3GapFill/>
            </template>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>

          <b-nav-item-dropdown right no-caret>
            <template v-slot:button-content>
              <BIconPersonCircle/>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
    </b-navbar>
  </div>
</template>

<script>
import { BIconGrid3x3GapFill, BIconPersonCircle } from 'bootstrap-vue'
export default {
  name: 'TopBar',
  components: {
    BIconGrid3x3GapFill,
    BIconPersonCircle
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
