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
  import { flag } from "./store.js";

  let FLAG = false;

  afterUpdate(() => {
    flag.subscribe((value) => {
      FLAG = value;
    });
  });

  function setFlag() {
    flag.update((n) => true);
  }

  import { onMount } from "svelte";

  onMount(async () => {
    AFRAME.registerComponent("log", {
      init: function () {
        this.el.addEventListener("timeout", () => {
          setFlag();
          alert()
        });
      },
    });

    setFlag();
  });
</script>

<a-scene id="gallery-scene" renderer="antialias: true">
  <a-assets log timeout="10000">
    <!-- 52 Portraits -->
    <img id="logo-image" alt="" src="portfolio/logo.png" />
    <img id="services-image" alt="" src="portfolio/service_1.png" />

    <!-- svelte-ignore a11y-media-has-caption -->
    <video
      id="intro-video"
      autoplay
      loop="true"
      alt=""
      src="portfolio/intro_New.mp4"
      type="video/mp4"
    />

    <!-- svelte-ignore a11y-media-has-caption -->
    <video
      id="colpo-gif"
      type="video/mp4"
      autoplay
      loop="true"
      src="portfolio/colpo.mp4"
    />

    <!-- svelte-ignore a11y-media-has-caption -->
    <video
      id="jananya-gif"
      type="video/mp4"
      autoplay
      loop="true"
      src="portfolio/jananya.mp4"
    />
    <!-- svelte-ignore a11y-media-has-caption -->
    <video
      id="bowel-gif"
      type="video/mp4"
      autoplay
      loop="true"
      src="portfolio/bowel retractor.mp4"
    />
    <img id="oral-gif" alt="" src="portfolio/oral.gif" />

    <img id="urowear-gif" alt="" src="portfolio/urowear gif.gif" />
    <img id="kidney-gif" alt="" src="portfolio/kidney function test.gif" />
    <img id="olemus-gif" alt="" src="portfolio/olemus gif.gif" />
    <img id="eye-gif" alt="" src="portfolio/eye.gif" />
    <img id="cpr-gif" alt="" src="portfolio/cpr.gif" />
    <img id="glu-gif" alt="" src="portfolio/glu.gif" />

    <!-- right wall images -->
    <img id="osmf-gif" alt="" src="portfolio/osmf.gif" />
    <!-- svelte-ignore a11y-media-has-caption -->
    <video
      id="nebiro-gif"
      type="video/mp4"
      autoplay
      loop="true"
      src="portfolio/nebiro.mp4"
    />
    <img id="arm-gif" alt="" src="portfolio/arm.gif" />
    <img id="bulb-gif" alt="" src="portfolio/bulb_idea.gif" />
    <img id="organ-gif" alt="" src="portfolio/organ.gif" />
    <img id="neuro-gif" alt="" src="portfolio/neuro.gif" />
    <img id="heart-gif" alt="" src="portfolio/heart.gif" />
    <img id="amtz" alt="" src="portfolio/amtz.jpg" />
    <img id="medivalley" alt="" src="portfolio/medivalley.png" />

    <!--back wall-->
    <img id="mouth-gif" alt="" src="portfolio/mouth.gif" />
    <img id="history" alt="" src="portfolio/history.png" />
    <img id="service_1" alt="" src="portfolio/services.png" />
    <img id="dental-gif" alt="" src="portfolio/dental.gif" />
    <img id="ear-gif" alt="" src="portfolio/ear.gif" />
    <img id="organ-gif" alt="" src="portfolio/organ.gif" />
    <img id="liquid-gif" alt="" src="portfolio/liquid.gif" />
    <!-- svelte-ignore a11y-media-has-caption -->
    <video
      id="tyro-gif"
      type="video/mp4"
      autoplay
      loop="true"
      src="portfolio/tyro.mp4"
    />

    <!-- Discarded -->
  </a-assets>
  {#if FLAG}
    <!-- content here -->
    <Lights />
    <Camera />

    <Front />
    <Left />
    <Right />
    <Back />
    <Floor />
    <Roof />
  {:else}
    <h2>Loading...</h2>
  {/if}
  <!-- Main light -->
</a-scene>
