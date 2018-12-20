# L.EasyButton - Edited from : https://github.com/CliffCloud/Leaflet.EasyButton
-----------------------------------------------------------------------------------
##### Hello World - USAGE 
```javascript
  var map = L.map('map').setView([35, -95], 4);
  var params = {
    layers: 'topp:states',
    format: 'image/png',
    transparent: true
  }
  L.tileLayer('http://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 18,
    attribution: 'Map data © <a href="http://openstreetmap.org">OpenStreetMap</a> contributors',
  }).addTo(map);
  
  var button = L.easyButton('fa-globe', function(btn, map){
      console.log('clicked');
  },
  function(btn, map){
      console.log('dataaa');
    });
  
  button.button.style.width = "50px";
  button.button.style.height = "50px";
  
  button.addTo( map );
```
