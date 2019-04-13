<html>
  <head>
    <title>Multiple Markers - A-Frame School</title>
    <meta name="description" content="Multiple Markers - A-Frame School">
    <script src="https://aframe.io/releases/0.7.0/aframe.min.js"></script>
    <!-- include ar.js for A-Frame -->
<script src="https://jeromeetienne.github.io/AR.js/aframe/build/aframe-ar.js"></script>

  </head>
<body style="margin : 0px; overflow: hidden;">
  <a-scene embedded arjs="sourceType: webcam;">
    <!-- handle marker with your own pattern -->
    <a-marker type="pattern" patternurl="markers/hiro-m.patt">
      <a-sphere position="0 0.5 0" radius="0.25" rotation="0 10 0" color="#EF2D5E"></a-sphere>
    </a-marker>
    <a-marker type="pattern" patternurl="kmarkers/kitten.patt">
      <a-sphere position="0 0.5 0" radius="0.25" rotation="0 10 0" color="#ffccff"></a-sphere>
    </a-marker>
    <!-- handle marker with hiro preset -->
    <a-marker preset="hiro">
      <a-box position="0 0.5 0" material="color: green;"></a-box>
    </a-marker>
    <!-- handle barcode marker -->
    <a-marker type="barcode" value="5">
      <a-box position="0 0.5 0" material="color: blue;"></a-box>
    </a-marker>
    <!-- add a simple camera -->
    <a-entity camera></a-entity>
  </a-scene>
</body>
</html>
