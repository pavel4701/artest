
<!doctype HTML>
<html>
<script src="https://aframe.io/releases/0.6.1/aframe.min.js"></script>
<script src="https://rawgit.com/donmccurdy/aframe-extras/master/dist/aframe-extras.loaders.min.js"></script>
<script src="https://cdn.rawgit.com/jeromeetienne/AR.js/1.5.0/aframe/build/aframe-ar.js"> </script>
  <body style='margin : 0px; overflow: hidden;'>
    <a-scene stats embedded arjs='trackingMethod: best;'>
    <a-assets>
      <a-asset-item id="smiley" src="https://cdn.rawgit.com/KhronosGroup/glTF-Sample-Models/9176d098/1.0/SmilingFace/glTF/SmilingFace.gltf"></a-asset-item>
    </a-assets>
  	<a-marker preset="hiro">
      <a-entity gltf-model="#smiley" rotation= "180 0 0">
      </a-entity>
  	</a-marker>
  	<a-entity camera></a-entity>
    </a-scene>
  </body>
</html>
