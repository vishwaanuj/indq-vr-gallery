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

  <a-marker type="pattern" url="./MARKERS/0.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/THE BEAT.glb"
      rotate="0 0 0"
      scale="20 10 20"
    >
    </a-entity>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/1.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/ORCHEST.glb"
      rotate="0 -10 0"
      scale="35 20 30"
    >
    </a-entity>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/2.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/bed.glb"
      rotate="0 -10 0"
      scale="1 .5  1"
    >
    </a-entity>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/3.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/IIT PAPER.glb"
      rotate="0 -10 0"
      scale="20 10 20"
    >
    </a-entity>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/4.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/IIT LIQUID.glb"
      rotate="0 -10 0"
      scale="20 10 20"
    >
    </a-entity>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/5.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/OLEMUS.glb"
      rotate="0 -10 0"
      scale="10 5 10"
    >
    </a-entity>
  </a-marker>
  <a-marker type="pattern" url="./MARKERS/6.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/thyrolemus.glb"
      rotate="0 -10 0"
      scale="1 .5 1"
    >
    </a-entity>
  </a-marker>
  <a-marker type="pattern" url="./MARKERS/7.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/NEBIRO.glb"
      rotate="0 -10 0"
      scale="10 5 10"
    >
    </a-entity>
  </a-marker>
  <a-entity camera></a-entity>
</a-scene>

<style>
</style>
