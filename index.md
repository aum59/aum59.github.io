<p align="center">
  <H1>Aum59 My Page</H1>
</p>
<p align="center"> 
  <img src="pictures/aumpic.jpg"/>
</p>

<br>

## [**อัลบั้มรูป**](myalbum.md)
## [**ประวัติการศึกษา**](education.md)
## [**ความสามารถพิเศษ**](ability.md)
## [**ผลงาน**](project.md)

<br>

* * *

### Social Network

*  Email : intarumpun@yahoo.com
*  FaceBook : /intarumpun
*  ID Line : intarumpun

<br>
<link rel="stylesheet" type="text/css" href="/css/mycss.css">

<div id="map" style="width:200px;height:200px"></div>

<script>
function myMap() {
  var myCenter = new google.maps.LatLng(14.599698,100.362549);
  var mapCanvas = document.getElementById("map");
  var mapOptions = {center: myCenter, zoom: 5};
  var map = new google.maps.Map(mapCanvas, mapOptions);
  var marker = new google.maps.Marker({position:myCenter});
  marker.setMap(map);
}
</script>

<script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyBu-916DdpKAjTmJNIgngS6HL_kDIKU0aU&callback=myMap"></script>
