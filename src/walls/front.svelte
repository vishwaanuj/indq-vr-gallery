<script>
</script>

<a-box width="102.5" height="85" depth="0.25" position="0 0 -15" color="#fff">
  <!-- Middle image: pancakes -->
  <a-entity position="-4 28 0.3">
    <a-image
      alt=""
      src="#logo-image"
      width="18"
      height="9"
      depth="0.15"
      position="0 0 0"
    />
    <a-text
      width="28"
      height="14"
      value="INNOVATION.DESIGN.QUOTIENT"
      position="-8.5 -7 .5"
    />
  </a-entity>

  <a-entity
    position="-7 0 0.3"
    style="border:dotted 8px white"
    animation__fusing="
                      property: position; 
                      startEvents: fusing; 
                      easing: easeInCubic;
                      dur: 1600; 
                      to:-7 0 14"
    animation__mouseleave="
                      property: position;
                      startEvents: mouseleave;
                      dir: alternate;
                      dur: 1000; 
                      to: -7 0 0.3"
  >
    <a-image src="#services-image" width="60" height="30" />


  </a-entity>

</a-box>

<!-- Right image: octopus -->
