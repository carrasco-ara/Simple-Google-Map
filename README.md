# Simple-Google-Map
<!-- Udacity Google's Maps - 5.Hello Map Lesson 1 - Getting Started with the APIs -->
<html>
 <head>
 <!-- styles put here, but you can include a CSS file and reference it instead! -->
   <style type="text/css">
      /* Always set the map height explicitly to define the size of the div
       * element that contains the map. */
      #map {
        height: 100%;
      }
      /* Optional: Makes the sample page fill the window. */
      html, body {
        height: 100%;
        margin: 0;
        padding: 0;
      }
   </style>
 </head>
 <body>
   <!-- display map here -->
   <div id="map"></div>
   <script>

	   // Create a new map instance  map=new google.maps.Map
     // 1) Where in the html to load the map  (document.getElementByID(‘map’),
     // 2) And where in the world to show. Center  and zoom 
     //    Center -  lat and lng
     //    Zoom – the higher the number the more detailed up to 21
     // TODO: use a constructor to create a new map JS object. You can use the coordinates
     // map 150 E. Colorado Blvd., Pasadena CA 91105 
      var map;
      function initMap() {
        map = new google.maps.Map(document.getElementById('map'), {
          center: {lat: 34.1456598, lng: -118.1461886},
          zoom: 13
        });
      }	 
   </script>
   <!--TODO: Load the JS API ASYNCHRONOUSLY below.-->
    <script async defer src="https://maps.googleapis.com/maps/api/js?key=AIzaSyDmIrWCMYK4r7LQ2f-pHGNtZ6RhK5C6uDE&v=3&callback=initMap" ></script>   
   <script>
   </script>
 </body>
</html>
