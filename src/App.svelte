<script>

</script>

<a-scene
  vr-mode-ui="enabled: false;"
  renderer="logarithmicDepthBuffer: true;"
  arjs="debugUIEnabled: false;sourceWidth:1280; sourceHeight:960; displayWidth: 1280; displayHeight: 960;"
>
  <a-assets timeout="20000">
    <a-asset-item id="dopplerModel" src="./GLB_MODELS/THE BEAT.glb"
    ></a-asset-item>
    <a-asset-item id="BED" src="./GLB_MODELS/bed.glb"></a-asset-item>
    <a-asset-item id="ORCHEST" src="./GLB_MODELS/ORCHEST.glb"></a-asset-item>
    <a-asset-item id="OLEMUS" src="./GLB_MODELS/OLEMUS.glb"></a-asset-item>
  </a-assets>

  <a-marker type="pattern" url="./MARKERS/0.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/THE BEAT.glb"
      rotate="0 0 0"
      scale="15 5 15"
      animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
         
    >
    </a-entity>
    <a-text value="Prenatal Doppler"  align="center" rotation="0 0 0" position="0 -1 0"
    ></a-text>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/1.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/ORCHEST.glb"
      rotate="0 -10 0"
      scale="25 5 20"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="ORCHEST STETHOSCOPE"  align="center" rotation="0 0 0" position="0 -1 0"
    ></a-text>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/2.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/bed.glb"
      rotate="0 -10 0"
      scale="1 .5  1"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="Hospital Bed"  align="center" rotation="0 0 0" position="0 -1 0"/>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/3.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/IIT PAPER.glb"
      rotate="0 -10 0"
      scale="20 10 20"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="Paper Assay Reader"  align="center" rotation="0 -90 0" position="0 -1 0"/>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/4.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/IIT LIQUID.glb"
      rotate="0 -10 0"
      scale="20 10 20"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="Liquid Assay Reader"  align="center" rotation="0 0 0" position="0 -1 0"/>
  </a-marker>

  <a-marker type="pattern" url="./MARKERS/5.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/OLEMUS.glb"
      rotate="0 -10 0"
      scale="10 5 10"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="Olemus"  align="center" rotation="0 0 0" position="0 -1 0"/>
  </a-marker>
  <a-marker type="pattern" url="./MARKERS/6.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/thyrolemus.glb"
      rotate="0 -10 0"
      scale="1 .5 1"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="Thyro Olemus"  align="center" rotation="0 0 0" position="0 -1 0"/>
  </a-marker>
  <a-marker type="pattern" url="./MARKERS/7.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/NEBIRO.glb"
      rotate="0 -10 0"
      scale="15 10 15"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="Nebiro"  align="center" rotation="0 0 0" position="0 -1 0"/>
  </a-marker>



  <a-marker type="pattern" url="./MARKERS/8.patt">
    <!-- White plane as a background for the text -->

    <a-entity
      gltf-model="./GLB_MODELS/JANANYA.glb"
      rotate="0 -10 0"
      position="0 -5 5"
      scale="25 20 25"
       animation="property: rotation; to: 0 360 0; loop: true; dur: 20000;"
    >
    </a-entity>
    <a-text value="Jananya"  align="center" rotation="0 0 0" position="0 -1 0"/>
  </a-marker>
  <a-entity camera></a-entity>
</a-scene>

<style>
</style>
