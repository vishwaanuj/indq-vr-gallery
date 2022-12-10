<a-entity position="-2 3 25">
  <a-entity camera look-controls wasd-controls>
    <a-entity position="0 0 -3"
              geometry="primitive: ring; radiusInner: 0.04; radiusOuter: 0.06;"
              material="color: gray; shader: flat"
              cursor="maxDistance: 30; fuse: true;fusetimeout:250">
      <a-animation begin="click" easing="ease-in" attribute="scale"
           fill="forwards" from="0.2 0.2 0.2" to="1 1 1" dur="150"></a-animation>
      <a-animation begin="fusing" easing="ease-in" attribute="scale"
           fill="backwards" from="1 1 1" to="0.2 0.2 0.2" dur="1500"></a-animation>
    </a-entity>
  </a-entity>
</a-entity>