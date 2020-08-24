<template>
  <div class="google-home">
    <TopBar/>
    <div class="vertical-spacer"></div>
    <div class="google-image">
      <img src="../assets/google-logo.png">
    </div>
    <b-container align="center">
      <b-col/>
      <b-col cols="10">
        <b-input-group class="searchBarGroup">
          <b-input-group-prepend class="searchIconLeft rounded-left">
            <BIconSearch/>
          </b-input-group-prepend>
          <b-form-input type="search" class="searchBar"></b-form-input>
          <b-input-group-append class="searchIconRight rounded-right">
            <BIconMic v-b-tooltip.hover.bottom title="Search by voice"/>
          </b-input-group-append>
        </b-input-group>
      </b-col>
      <b-col/>
    </b-container>
    <b-button class="google-button">Google Search</b-button>
    <b-button class="google-button">I'm Feeling Lucky</b-button>
    <div class="languages">
      Google offered in:
      <b-link>Afrikaans</b-link>
      <b-link>Sesotho</b-link>
      <b-link>isiZulu</b-link>
      <b-link>IsiXhosa</b-link>
      <b-link>Setswana</b-link>
      <b-link>Northern Sotho</b-link>
    </div>
    <BottomBar/>
  </div>
</template>

<script>
import TopBar from '@/components/TopBar';
import BottomBar from '@/components/BottomBar';
import { BIconSearch, BIconMic } from 'bootstrap-vue';

export default {
  name: 'GoogleHome',
  components: {
    TopBar,
    BIconSearch,
    BIconMic,
    BottomBar,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.google-home {
  height: 100%;
}

.google-button {
  background-image: -webkit-linear-gradient(top, #f5f5f5, #f1f1f1);
  background-color: #f2f2f2;
  border: 1px solid #f2f2f2;
  border-radius: 4px;
  color: #5F6368;
  font-family: arial, sans-serif;
  font-size: 14px;
  margin: 11px 4px;
  padding: 0 16px;
  line-height: 27px;
  height: 36px;
  min-width: 54px;
  text-align: center;
  cursor: pointer;
  user-select: none;
}

.searchBar {
  border-left: none;
  border-right: none;
}

.searchIconLeft {
  display: flex;
  align-items: center;
  padding-left: 0.375rem;
  padding-right: 0.375rem;
  margin-bottom: 0;
  /*font-size: 1rem;*/
  /*font-weight: 400;*/
  /*line-height: 1.5;*/
  color: #495057;
  text-align: center;
  white-space: nowrap;
  background-color: white;
  border-bottom: 1px solid #ced4da;
  border-top: 1px solid #ced4da;
  border-left: 1px solid #ced4da;
  /*border-radius: 0.25rem;*/
}

.searchIconRight {
  display: flex;
  align-items: center;
  padding-left: 0.375rem;
  padding-right: 0.375rem;
  margin-bottom: 0;
  /*font-size: 1rem;*/
  /*font-weight: 400;*/
  /*line-height: 1.5;*/
  color: #495057;
  text-align: center;
  white-space: nowrap;
  background-color: white;
  border-bottom: 1px solid #ced4da;
  border-top: 1px solid #ced4da;
  border-right: 1px solid #ced4da;
  /*border-radius: 0.25rem;*/
}

.vertical-spacer {
  height: 120px;
}

.google-image {
  padding: 20px;
}

.searchBarGroup {
  padding-top: 10px;
  padding-bottom: 10px;
}

.languages {
  padding-top: 10px;
  padding-bottom: 10px;
  font-size: small;
}

.languages a {
  padding-right: 3px;
  padding-left: 3px;
}

.footer {
  width: 100%;
  height: 100%;
}

</style>
