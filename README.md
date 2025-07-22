<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Colonias y Maquillaje</title>

  <!-- ✅ Metaetiqueta de verificación de Google -->
  <meta name="google-site-verification" content="CyYLSySfE0_wZemfSaUlymLf4k21z9AsoJJP6Mb9wrY" />

  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #fff0f5;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #ffb6c1;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    .productos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
      padding: 2rem;
    }
    .producto {
      background-color: white;
      padding: 1rem;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: center;
    }
    .producto img {
      width: 100%;
      border-radius: 8px;
    }
    .boton {
      background-color: #ff69b4;
      color: white;
      border: none;
      padding: 0.5rem 1rem;
      margin-top: 0.5rem;
      cursor: pointer;
      border-radius: 5px;
    }
    footer {
      background-color: #ffb6c1;
      color: white;
      text-align: center;
      padding: 1rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Bienvenida a Colonias y Maquillaje</h1>
    <p>Encuentra productos de belleza y fragancias únicas</p>
  </header>

  <section class="productos">
    <div class="producto">
      <img src="https://cdn.pixabay.com/photo/2016/11/22/20/03/woman-1853272_1280.jpg" alt="Maquillaje mujer elegante" />
      <h3>Paleta de sombras profesional</h3>
      <button class="boton" onclick="location.href='https://wa.me/34624387627'">Encargar por WhatsApp</button>
    </div>
    <div class="producto">
      <img src="https://cdn.pixabay.com/photo/2017/08/06/19/03/perfume-2593485_1280.jpg" alt="Perfume elegante" />
      <h3>Colonia floral 100ml</h3>
      <button class="boton" onclick="location.href='https://wa.me/34624387627'">Encargar por WhatsApp</button>
    </div>
    <!-- Puedes duplicar estos bloques y cambiar imagen/nombre del producto -->
  </section>

  <footer>
    <p>Contáctanos al WhatsApp +34 624 387 627</p>
  </footer>
</body>
</html>
