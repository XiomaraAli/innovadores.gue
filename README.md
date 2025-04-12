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

    <a href="juego.html"><button>Jugar</button></a>
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
