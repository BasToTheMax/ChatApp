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
    <sub>Praat hier over algemene dingen</sub>
  </div>
</div>

<div class="w3-container w3-hover">
  <img src="{{ site.base }}/profile.jpg" style="max-width: 30px;">
  <p>Hallo! Hoe gaat het?</p>
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
