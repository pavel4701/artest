<html>
<head>
  <script src="https://aframe.io/releases/0.6.0/aframe.min.js"></script>

  <script src="https://jeromeetienne.github.io/AR.js/aframe/build/aframe-ar.js"></script>
</head>
<body style='margin : 0px; overflow: hidden;'>
    <a-scene embedded arjs='trackingMethod: best; debugUIEnabled:false'>
        <a-assets>
            <a-asset-item id="tree-model" src="https://raw.githubusercontent.com/pavel4701/artest/master/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.dae" crossOrigin="anonymous"></a-asset-item>
            <a-asset-item id="text-model" src="https://raw.githubusercontent.com/pavel4701/artest/master/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.dae" crossOrigin="anonymous"></a-asset-item>
       </a-assets>
        <a-marker preset='custom' type='pattern' url='https://raw.githubusercontent.com/pavel4701/pattern-marker./master/pattern-marker%20(6).patt'>
<---display first model     --->
<a-entity collada-model="#tree-model"></a-entity>

         </a-marker>
         <a-entity camera></a-entity>
    </a-scene>
</body>
</html>
