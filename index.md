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

<div align="center">
  <p id="demo"></p>
  <h3 onclick="getLocation()"><i>You're around this :)b</i></h3>
  <div id="mapgoogle"></div>  
</div>

<script>
var x = document.getElementById("demo");

function getLocation() {
    if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(showPosition, showError);
    } else {
        x.innerHTML = "Geolocation is not supported by this browser.";
    }
}

function showPosition(position) {
    var latlon = position.coords.latitude + "," + position.coords.longitude;
    
    var img_url = "https://maps.googleapis.com/maps/api/staticmap?center="
    +latlon+"&zoom=14&size=400x300&sensor=false&key=AIzaSyBu-916DdpKAjTmJNIgngS6HL_kDIKU0aU";
    document.getElementById("mapholder").innerHTML = "<img src='"+img_url+"'>";   

}

function showError(error) {
    switch(error.code) {
        case error.PERMISSION_DENIED:
            x.innerHTML = "User denied the request for Geolocation."
            break;
        case error.POSITION_UNAVAILABLE:
            x.innerHTML = "Location information is unavailable."
            break;
        case error.TIMEOUT:
            x.innerHTML = "The request to get user location timed out."
            break;
        case error.UNKNOWN_ERROR:
            x.innerHTML = "An unknown error occurred."
            break;
    }
}
</script>
