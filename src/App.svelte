<script>
  import svelteLogo from "./assets/svelte.svg";
  import viteLogo from "/vite.svg";

  import Counter from "./lib/Counter.svelte";
  import pattern from "./assets/svelte.svg";

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
  <a-assets timeout="7000">
   
    <img id="osmf-gif" alt="" src="./osmf.gif" />
  </a-assets>
  <a-marker type="pattern" url="./0.patt">
    <!-- White plane as a background for the text -->
   
      
    <a-entity  shadow="cast: true" gltf-model="./doppler.glb" position="0 0 -20" scale="0.5 0.5 0.5" ><a-entity/>
   
 

    <!-- a-text positioned on the white plane -->
  </a-marker>

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
