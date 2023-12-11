<script>
  import svelteLogo from "./assets/svelte.svg";
  import viteLogo from "/vite.svg";
 
  import Counter from "./lib/Counter.svelte";
  import pattern from "./assets/svelte.svg";

</script>

<a-scene
  vr-mode-ui="enabled: false;"
  renderer="logarithmicDepthBuffer: true;"
  arjs="debugUIEnabled: false;sourceWidth:1280; sourceHeight:960; displayWidth: 1280; displayHeight: 960;"
>
  <!-- a-nft is the anchor that defines an Image Tracking entity -->
  <!-- on 'url' use the path to the Image Descriptors created before. -->
  <!-- the path should end with the name without the extension e.g. if file is trex.fset' the path should end with trex -->
  <a-nft
    type="nft"
    url="./LOGO_DESC/logo_b"
    smooth="true"
    smoothCount="1"
    smoothTolerance=".01"
    smoothThreshold="5"
  >
    <!-- as a child of the a-nft entity, you can define the content to show. here's a GLTF model entity -->
    <a-entity
      gltf-model="doppler.gltf"
      scale="5 5 5"
      position="100 10 0"
    >
    </a-entity>
  </a-nft>
  <!-- static camera that moves according to the device movemenents -->
  <a-entity camera></a-entity>
</a-scene>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
  .read-the-docs {
    color: #888;
  }
</style>
