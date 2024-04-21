<!DOCTYPE html>
<html>
<head>
  <title>Obyek 3D dengan A-Frame</title>
  <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
  <script src="https://cdn.rawgit.com/jeromeetienne/AR.js/2.0.8/aframe/build/aframe-ar.js"></script>
</head>
<body style="margin: 0px; overflow: hidden;">
  <a-scene embedded vr-mode-ui="enabled: false" arjs="debugUIEnabled: false;">
    <a-marker-camera preset="hiro">
      <!-- Obyek 1: Kotak -->
      <a-box position="-5 1.5 -10" color="#FF5733" scale="1 2 1"></a-box>

      <!-- Obyek 2: Silinder -->
      <a-cylinder position="5 1.25 -10" radius="1" height="2" color="#3498DB"></a-cylinder>

      <!-- Obyek 3: Kerucut -->
      <a-cone position="0 1.25 -15" radius-bottom="1" radius-top="0" height="2" color="#2ECC71" rotation="0 45 0"></a-cone>

      <!-- Obyek 4: Dodecahedron -->
      <a-dodecahedron position="-10 1.5 -15" radius="1" color="#9B59B6"></a-dodecahedron>

      <!-- Obyek 5: Sphere -->
      <a-sphere position="10 1.25 -15" radius="1.25" color="#E74C3C" material="metalness: 0.5; roughness: 0.5;"></a-sphere>
    </a-marker-camera>

    <!-- Kamera AR -->
    <a-entity camera arjs-anchor look-controls></a-entity>
  </a-scene>
</body>
</html>
