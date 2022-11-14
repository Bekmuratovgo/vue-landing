<template>
  <div class="App">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Main from './page/Main.vue';
import Footer from './components/Footer/Footer.vue';
import Header from './components/Header/Header.vue';
export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
  }
}
</script>

<style>
*{
  font-family: 'Montserrat';
}
.App {
  display: flex;
  flex-direction: column;
  align-content: space-between;
  width: 100%;
}
body {
  margin: 0;
}
@media screen and (max-width: 320px) {
  html {
    width: 100%;
  }
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
  display: flex;
  justify-content: center;
}
</style>
