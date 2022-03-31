<template>
  <HeaderApp/>
  <AreaConteudo/>
</template>

<script>
import HeaderApp from "./components/HeaderApp.vue"
import AreaConteudo from "./components/AreaConteudo.vue"
export default {
  name: 'App',
  components: {
    HeaderApp,
    AreaConteudo
  }
}
</script>

<style>
*{
margin: 0;
padding: 0;
}
body{
  margin: 0px;
  padding: 0px;
  background-color: #5a5a5a;
  color: white;
}
</style>
