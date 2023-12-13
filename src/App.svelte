<script>
  // Define the URL for Doppler 3D model
  const dopplerModelUrl = "./doppler.gltf";

  const markerPosition = { x: 0, y: 0, z: 200 };
  const textSize = { x: 1.5, y: 1.5, z: 1.5 };
</script>

<a-scene
  vr-mode-ui="enabled: false;"
  renderer="logarithmicDepthBuffer: true;"
  arjs="debugUIEnabled: false;sourceWidth:1280; sourceHeight:960; displayWidth: 1280; displayHeight: 960;"
>
  <a-assets timeout="20000">
    <a-asset-item id="dopplerModel" src="./doppler.gltf"></a-asset-item>
  </a-assets>

  <a-marker type="pattern" url="./0.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./orchest.glb"
      rotate="0 -10 0"
      scale=".3 .3 .3"
    >
    </a-entity>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/1.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/JANANYA.glb"
      rotate="0 -10 0"
      scale="30 30 30"
    >
    </a-entity>
  </a-marker>

  <a-entity camera></a-entity>
</a-scene>

<style>
</style>
