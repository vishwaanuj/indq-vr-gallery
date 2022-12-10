<script>

let items=["#mouth-gif","#organ-gif","#liquid-gif","#ear-gif","#dental-gif"]
let pos=["-20.75 -1.5 0.8","-1.25 -1.5 0.85","40.75 -1.5 0.85",
"-20.75 15.5 0.8","40.25 15.5 0.8"]

</script>


<a-box
width="110"
height="85"
depth="0.25"
position="0 0 95"
rotation="0 180 0"
color="#fff">


<a-image 
src="#history"
width="35"
height="18"
depth="0.1"
position="9.75 15.5 0.85"
  animation__fusing="property: position; 
    startEvents: fusing; 
    easing: easeInCubic;
    dur: 1000; 
    to: 10 -1.5 45"
  animation__mouseleave="
    property:position;
    startEvents:mouseleave;
    dir:alternate;
    dur: 1000; 
    to:9.75 15.5 0.85"
  animation__fusing__2="property: scale; 
startEvents: fusing; 
easing: easeInCubic;
dur: 1000; 
to:1.8 1.4 1"
  animation__mouseleave__2="
property:scale;
startEvents:mouseleave;
dir:alternate;
dur: 1000; 
to:1 1 1"/>
{#each items as item,i}
<a-image
  src={item}
  width="18"
  height="12"
  depth="0.1"
  position={pos[i]}
  material="shader:gif"
    animation__fusing="property: position; 
      startEvents: fusing; 
      easing: easeInCubic;
      dur: 1000; 
      to: 10 -1.5 45"
    animation__mouseleave="
      property:position;
      startEvents:mouseleave;
      dir:alternate;
      dur: 1000; 
      to:{pos[i]}"
    animation__fusing__2="property: scale; 
  startEvents: fusing; 
  easing: easeInCubic;
  dur: 1000; 
  to:1.8 1.2 1"
    animation__mouseleave__2="
  property:scale;
  startEvents:mouseleave;
  dir:alternate;
  dur: 1000; 
  to:1 1 1"
  />
   <!-- content here -->
{/each}
<a-video
  src="#tyro-gif"
  width="18"
  height="12"
  depth="0.1"
  position="19.75 -1.5 0.85"
    animation__fusing="property: position; 
      startEvents: fusing; 
      easing: easeInCubic;
      dur: 1000; 
      to: 10 -1.5 45"
    animation__mouseleave="
      property:position;
      startEvents:mouseleave;
      dir:alternate;
      dur: 1000; 
      to:19.75 -1.5 0.85"
    animation__fusing__2="property: scale; 
  startEvents: fusing; 
  easing: easeInCubic;
  dur: 1000; 
  to:1.8 1.2 1"
    animation__mouseleave__2="
  property:scale;
  startEvents:mouseleave;
  dir:alternate;
  dur: 1000; 
  to:1 1 1"
  />

</a-box>