<template>
  <div id="app">
    <b-container fluid class="bv-example-row bv-example-row-flex-cols">
      <b-row align-v="start">
        <b-col cols="12">
          <Header/>
        </b-col>
      </b-row>
      <b-row align-v="stretch">
        <router-view />
      </b-row>
    </b-container>
  </div>
</template>

<script>
import "bootstrap/dist/css/bootstrap.css";
import "bootstrap-vue/dist/bootstrap-vue.css";
import Header from "@/components/header";

export default {
  name: "App",
  components : {Header}
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
