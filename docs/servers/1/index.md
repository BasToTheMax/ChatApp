<!-- Sidebar -->
<div class="w3-sidebar w3-bar-block" style="display:none" id="mySidebar">
  <button onclick="w3_close()" class="w3-bar-item w3-button w3-large">Close &times;</button>
  <p> ! - ALLEEN LEZEN</p>
  <a href="{{ page.path }}/channels/1" class="w3-bar-item w3-button w3-blue"># Algemeen</a>
  <a href="{{ page.path }}/channels/2" class="w3-bar-item w3-button"># Regels</a>
  <a href="{{ page.path }}/channels/3" class="w3-bar-item w3-button"># Updates</a>
</div>

<!-- Page Content -->
<div class="w3-teal">
  <button class="w3-button w3-teal w3-xlarge" onclick="w3_open()">☰</button>
  <div class="w3-container">
    <h1># Algemeen</h1>
    <sup>Praat hier over algemene dingen</sup>
  </div>
</div>

<div id="msg"></div>
<div class="w3-container w3-hover">
  <img src="{{ site.base }}/profile.jpg" style="max-width: 40px;">
  <p>Hallo! Hoe gaat het?</p>
  <hr>
</div>

<script>
function w3_open() {
  document.getElementById("mySidebar").style.width = "80%";
  document.getElementById("mySidebar").style.display = "block";
}

function w3_close() {
  document.getElementById("mySidebar").style.display = "none";
}
</script>

script>
var cars = ["Hoi", "Max is een kat!"];
var text = "";
var i;
for (i = 0; i < cars.length; i++) {
  text += "<div class=\"w3-container w3-hover\"><img src=\"{{ site.base }}/profile.jpg\" style=\"max-width: 40px;\"><p>" + cars[i] + "</p><hr></div><br>";
}
document.getElementById("msg").innerHTML = text;
</script>
