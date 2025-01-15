# Mi Blog

¡Bienvenidos a mi blog! Aquí compartiré mis ideas, proyectos y más.

## Primer Post

Este es mi primer post en GitHub Pages. ¡Espero que disfrutes el contenido!


## Pestañas

<div class="tabs">
  <button class="tablinks" onclick="openTab(event, 'Tab1')">Pestaña 1</button>
  <button class="tablinks" onclick="openTab(event, 'Tab2')">Pestaña 2</button>
  <button class="tablinks" onclick="openTab(event, 'Tab3')">Pestaña 3</button>
</div>

<div id="Tab1" class="tabcontent">
  <h3>Pestaña 1</h3>
  <p>Contenido de la primera pestaña.</p>
</div>

<div id="Tab2" class="tabcontent">
  <h3>Pestaña 2</h3>
  <p>Contenido de la segunda pestaña.</p>
</div>

<div id="Tab3" class="tabcontent">
  <h3>Pestaña 3</h3>
  <p>Contenido de la tercera pestaña.</p>
</div>

<script>
function openTab(evt, tabName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(tabName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>
