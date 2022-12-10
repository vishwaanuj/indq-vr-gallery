<script>
  import { afterUpdate } from "svelte";
  import Front from "./walls/front.svelte";
  import Floor from "./walls/floor.svelte";
  import Roof from "./walls/roof.svelte";
  import Left from "./walls/left.svelte";
  import Right from "./walls/right.svelte";
  import Back from "./walls/back.svelte";
  import Assets from "./assets.svelte";
  import Lights from "./lights.svelte";
  import Camera from "./camera.svelte";

  afterUpdate(() => {
    window.addEventListener("click", function () {
      document.querySelector("#intro-video").play();
    });
  });
</script>

<a-scene id="gallery-scene" renderer="antialias: true">
  <Assets />

  <!-- Main light -->
  <Lights />
  <Camera />

  <Front />
  <Left />
  <Right />
  <Back />
  <Floor />
  <Roof />
</a-scene>
