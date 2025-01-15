<style>
/* Estilos del menú de navegación */
.navbar {
  overflow: hidden;
  background-color: #333;
  position: sticky;
  top: 0;
  width: 100%;
  display: flex;
  justify-content: center;
  margin: 0; /* Elimina márgenes */
  padding: 0; /* Elimina relleno extra */
  z-index: 1000; /* Asegura que esté encima de otros elementos */
}

.navbar a {
  float: left;
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  transition: background-color 0.3s;
}

.navbar a:hover {
  background-color: #575757;
}

/* Estilo de las secciones */
.section {
  display: none;
  padding: 20px;
}

.section.active {
  display: block;
}
</style>

<div class="navbar">
  <a href="#" onclick="switchSection('inicio')">Inicio</a>
  <a href="#" onclick="switchSection('proyectos')">Proyectos</a>
  <a href="#" onclick="switchSection('contacto')">Contacto</a>
</div>

<div id="inicio" class="section active">
  <h1>Inicio</h1>
  <p>¡Bienvenidos a mi blog! Aquí compartiré mis ideas, proyectos y más.</p>
</div>

<div id="proyectos" class="section">
  <h1>Proyectos</h1>
  <p>Esta es la sección de proyectos. Aquí puedes encontrar algunos de mis trabajos recientes.</p>
</div>

<div id="contacto" class="section">
  <h1>Contacto</h1>
  <p>Si quieres ponerte en contacto conmigo, envíame un mensaje a [mi correo](mailto:correo@example.com).</p>
</div>

<script>
function switchSection(sectionId) {
  var sections = document.getElementsByClassName("section");
  for (var i = 0; i < sections.length; i++) {
    sections[i].classList.remove("active");
  }
  document.getElementById(sectionId).classList.add("active");
}
</script>
