<template>
  <div id="app">
    <TitleTest />
    <AppJumbotron />
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />

    <a class="my-link" href="">Link</a>
    <button class="my-btn">Bottone</button>
  </div>
</template>

<script>
import TitleTest from "./components/TitleTest.vue";
import AppJumbotron from "./components/AppJumbotron.vue";

export default {
  name: "App",
  components: {
    TitleTest,
    AppJumbotron,
  },
};
</script>

<style lang="scss">
@import "./style/variable.scss";
@import "./style/common.scss";
@import "./style/mins.scss";

.primary-title {
  background-color: $brand-primary-color;
  color: $brand-secondary-color;
  padding: 0.5rem;
}

.secondary-title {
  background-color: $brand-secondary-color;
  color: $brand-primary-color;
}

a.my-link {
  @include app-button();
  color: lightcoral;
  background-color: yellow;
}

button.my-button {
  @include app-button();
}
// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }
</style>
