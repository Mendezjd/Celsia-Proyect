# Celsia-Proyect
<!doctype html>
<html lang="en">
  <head>
    <title><model-viewer> template</title>
    <meta charset="utf-8">
    <meta name="description" content="<model-viewer> template">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link type="text/css" href="./styles.css" rel="stylesheet"/>
  </head>
  <body>
    <model-viewer
      src="LogoCelsiaGLB3.glb"
      ios-src="LogoCelsiaUSDZ.usdz"
      ar
      ar-modes="scene-viewer webxr quick-look"
      camera-controls
      tone-mapping="neutral"
      poster="poster.webp"
      shadow-intensity="1">
      
      <div class="progress-bar hide" slot="progress-bar">
          <div class="update-bar"></div>
      </div>
      
      <button slot="ar-button" id="ar-button">
          View in your space
      </button>
      
      <div id="ar-prompt">
          <img src="ar_hand_prompt.png">
      </div>
    </model-viewer>  

    <!-- Carga model-viewer primero -->
    <script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/4.0.0/model-viewer.min.js"></script>
    <script src="script.js"></script>
  </body>
</html>
