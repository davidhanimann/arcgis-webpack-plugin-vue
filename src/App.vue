<template>
  <div id="app">
    <esri-map />
  </div>
</template>
<script>

import EsriMap from './Map'

export default {
  name: 'app',
  components: { EsriMap }
}
</script>

<style>
  body, html, div, #app {
    padding: 0;
    margin: 0;
    width: 100%;
    height: 100%;
  }
</style>
