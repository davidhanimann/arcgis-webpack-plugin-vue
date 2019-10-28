<template>
    <div id="mapViewDiv"></div>
</template>
<script>
import Map from "esri/Map";
import MapView from 'esri/views/MapView';
import geometryJsonUtils from 'esri/geometry/support/jsonUtils';
import geometryEngine from 'esri/geometry/geometryEngine';

export default {
  data() {
    return {
        mapView: null
    };
  },
  methods: {
    loadMap() {
        console.log(geometryJsonUtils)
        console.log(geometryEngine)
            this.mapView = new MapView({
              container: "mapViewDiv",
              map: new Map({ basemap: 'oceans' }),
              center: [-107.8, 37.3]
            });
    }
  },
  mounted () {
      this.loadMap();
  },

};
</script>
