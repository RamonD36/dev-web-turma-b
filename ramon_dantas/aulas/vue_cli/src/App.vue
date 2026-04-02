<template>
  <div>
    <img alt="Vue logo" src="./assets/logo.png" />
    <h1>Meu Primeiro APP Vue</h1>
    <HomeComponent />
    <hr>
    <UsuarioComponent />
    <hr>
    <EstiloComponente />
  </div>
</template>

<script>
import HomeComponent from "./components/HomeComponent.vue";
import UsuarioComponent from "./components/UsuarioComponent.vue";
import EstiloComponente from "./components/EstiloComponente.vue";

export default {
  name: "App",
  components: {
    HomeComponent,
    UsuarioComponent,
    EstiloComponente,
  },
  created() {
    console.log("Created");
  },
  mounted() {
    console.log("Mounted");
  },
  errorCaptured() {
    console.log("errorCaptured");
  },
};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
