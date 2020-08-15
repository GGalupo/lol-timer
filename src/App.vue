<template>
  <div id="app">
      <Header />
      <Main />
      <Footer />
  </div>
</template>

<script>
import Header from "./components/Header";
import Footer from "./components/Footer";
import Main from "./main/Main";

export default {
  name: "App",
  components: { Header, Footer, Main },
};
</script>

<style>
* {
  box-sizing: border-box;
  font-family: 'Lato', sans-serif;
}

body, html {
  margin: 0;
  padding: 0;
}

#app {
  /* background: linear-gradient(to right, #42275a, #734b6d); */
  background-color: #42275abb;
  
  height: 100vh;

  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 80px 1fr 60px;
  grid-template-areas:
    "header"
    "main"
    "footer";
}
</style>
