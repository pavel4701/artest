<!doctype HTML>
<html>
    <head>
        <meta name="viewport" content="width=device-width, user-scalable=no, minimum-scale=1.0, maximum-scale=1.0">
    </head>
    <script src="https://aframe.io/releases/0.9.0/aframe.min.js"></script>
    <script src="https://rawgit.com/jeromeetienne/AR.js/master/aframe/build/aframe-ar.min.js"></script>
    <script src="https://rawgit.com/donmccurdy/aframe-extras/master/dist/aframe-extras.loaders.min.js"></script>
    
    <body style='margin : 0px; overflow: hidden;'>
        <!-- we add detectionMode and matrixCodeType to tell AR.js to recognize barcode markers -->
        <a-scene embedded arjs='sourceType: webcam; debugUIEnabled: false; detectionMode: mono_and_matrix; matrixCodeType: 3x3;'>


            <a-asset-item id="animated-asset" src="https://raw.githubusercontent.com/pavel4701/artest/master/%D0%91%D0%B5%D0%B7%20%D0%BD%D0%B0%D0%B7%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.dae"></a-asset-item>

        <a-marker preset='custom' type='pattern' url='https://raw.githubusercontent.com/pavel4701/pattern-marker./master/pattern-marker%20(6).patt'>
            <a-box position='0 0.5 0' color="yellow"></a-box>
        </a-marker>
		
		  <a-marker id="animated-marker" type='barcode' value='6'>
            <a-entity
                gltf-model="#animated-asset"
                scale="2">
            </a-entity>
        </a-marker>

        <!-- use this <a-entity camera> to support multiple-markers, otherwise use <a-marker-camera> instead of </a-marker> -->
        <a-entity camera></a-entity>
        </a-scene>
    </body>
</html>
