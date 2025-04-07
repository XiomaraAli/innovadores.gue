<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Sendero del Sol - Juego</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="menu">
    <h1>SENDERO DEL SOL</h1>
    <p>Juego educativo: Historia del Perú</p>

    <button onclick="empezarJuego()">Jugar</button>
    <button onclick="mostrarInstrucciones()">Instrucciones</button>
    <button onclick="mostrarCreditos()">Créditos</button>
  </div>

  <div class="seccion" id="instrucciones" style="display: none;">
    <h2>Instrucciones</h2>
    <p>Explora, responde preguntas y gana puntos. ¡No caigas en las trampas!</p>
    <button onclick="volverMenu()">Volver al menú</button>
  </div>

  <div class="seccion" id="creditos" style="display: none;">
    <h2>Créditos</h2>
    <p>Desarrollado por el equipo Innovadores Granate.</p>
    <button onclick="volverMenu()">Volver al menú</button>
  </div>

  <script src="script.js"></script>
</body>
</html>

body {
  font-family: 'Segoe UI', sans-serif;
  background-color: #8B0000; /* granate */
  color: #fff;
  text-align: center;
  padding-top: 80px;
}

h1 {
  font-size: 48px;
  margin-bottom: 10px;
}

.menu p {
  font-size: 20px;
  margin-bottom: 30px;
}

button {
  padding: 12px 24px;
  font-size: 18px;
  margin: 10px;
  background-color: #fff;
  color: #8B0000;
  border: none;
  border-radius: 10px;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  background-color: #ffc107;
  color: #000;
}

.seccion {
  display: none;
}


function empezarJuego() {
  alert("¡Aquí irá tu juego! Puedes cambiar esta función para que inicie el juego real.");
  // window.location.href = "juego.html"; // si tienes otra página
}

function mostrarInstrucciones() {
  document.querySelector(".menu").style.display = "none";
  document.getElementById("instrucciones").style.display = "block";
}

function mostrarCreditos() {
  document.querySelector(".menu").style.display = "none";
  document.getElementById("creditos").style.display = "block";
}

function volverMenu() {
  document.querySelector(".menu").style.display = "block";
  document.getElementById("instrucciones").style.display = "none";
  document.getElementById("creditos").style.display = "none";
}
