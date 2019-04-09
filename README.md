<html>
<head>
  <script src="https://aframe.io/releases/0.6.0/aframe.min.js"></script>

  <script src="https://jeromeetienne.github.io/AR.js/aframe/build/aframe-ar.js"></script>
</head>
<body style='margin : 0px; overflow: hidden;'>
    <a-scene embedded arjs='trackingMethod: best; debugUIEnabled:false'>
        <a-assets>
            <a-scene>
   <a-entity id="box" geometry="primitive: box" material="color: red"></a-entity>
	<a-box color="red" rotation="0 45 45" scale="2 2 2"></a-box>
	<a-box color="red" position="0 2 -5" rotation="0 45 45" scale="2 2 2"></a-box>
  </a-scene>
  <a-scene>
        <a-marker preset='custom' type='pattern' url='https://raw.githubusercontent.com/pavel4701/pattern-marker./master/pattern-marker%20(6).patt'>
<---display first model     --->
<a-entity collada-model="#tree-model"></a-entity>

         </a-marker>
         <a-entity camera></a-entity>
    </a-scene>
</body>
</html>
