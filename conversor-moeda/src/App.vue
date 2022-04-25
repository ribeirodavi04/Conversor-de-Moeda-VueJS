<template>
  <div id="app">
    <div class="row">
      <ConversorMoeda moeda-a="USD" moeda-b="BRL"/>
      <ConversorMoeda moeda-a="BRL" moeda-b="USD"/>
    </div>
    
    <div class="row">
      <ConversorMoeda moeda-a="CAD" moeda-b="BRL"/>
      <ConversorMoeda moeda-a="BRL" moeda-b="CAD"/>
    </div>
    
    <div class="row">
      <ConversorMoeda moeda-a="EUR" moeda-b="BRL"/>
      <ConversorMoeda moeda-a="BRL" moeda-b="EUR"/>
    </div>
    
  </div>
</template>

<script>
import ConversorMoeda from './components/ConversorMoeda.vue'
export default {
  name: 'App',
  components: {
    ConversorMoeda
}
}
</script>

<style>
#app {
  max-width: 900px;
  margin: auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.row{
  display: flex;
  justify-content: space-around;
  margin-top: 40px;
}
</style>
