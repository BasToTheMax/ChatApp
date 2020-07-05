<!-- Sidebar -->
<div class="w3-sidebar w3-bar-block" style="display:none" id="mySidebar">
  <button onclick="w3_close()" class="w3-bar-item w3-button w3-large">Close &times;</button>
  <p> ! - ALLEEN LEZEN</p>
  <a href="{{ site.base }}/servers/1" class="w3-bar-item w3-button w3-blue"># Algemeen</a>
</div>

<!-- Page Content -->
<div class="w3-teal">
  <button class="w3-button w3-teal w3-xlarge" onclick="w3_open()">☰</button>
  <div class="w3-container">
    <h1># Algemeen</h1>
    <sup>Praat hier over algemene dingen</sup>
  </div>
</div>

<div id="msg">LOADING</div>
<!--

<div class="w3-container w3-hover">
  <img src="{{ site.base }}/profile.jpg" style="max-width: 40px;">
  <span>BasToTheMax</span>
  <p>Hallo! Hoe gaat het?</p>
  <hr>
</div>
-->


<script>
function w3_open() {
  document.getElementById("mySidebar").style.width = "80%";
  document.getElementById("mySidebar").style.display = "block";
}

function w3_close() {
  document.getElementById("mySidebar").style.display = "none";
}

var cars = ["Hoi", "Max is een kat!", "Oke", "Hhahah", "Lool", "Gu", "Llallala", "Test", "Discord"];
var text = "";
var i;
var user;
for (i = 0; i < cars.length; i++) {
  user = Math.floor(Math.random() * 6);
 
 switch(user) {
  case 0:
   name = 'Hoi';
    break;
  case 1:
    name = 'Katten zijn lief';
    break;
  default:
    name = 'USER';
}
 
 
  text += "<div class=\"w3-container w3-hover\"><img src=\"/ChatApp/profile.jpg\" style=\"max-width: 40px;\"><span>" + name + "</span><p>" + cars[i] + "</p><hr></div><br>";
}
document.getElementById("msg").innerHTML = text;
</script>
