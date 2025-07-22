
  
      <!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mi Tienda de Cosmética</title>
  <style><meta name="google-site-verification" content="CyYLSySfE0_wZemfSaUlymLf4k21z9AsoJJP6Mb9wrY" />
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #fff0f5;
      color: #333;
    }
    header {
      background: #d6336c;
      color: white;
      padding: 30px;
      text-align: center;
      font-size: 2em;
    }
    section {
      max-width: 1000px;
      margin: 40px auto;
      padding: 0 20px;
    }
    .product {
      background: white;
      border-radius: 15px;
      box-shadow: 0 8px 20px rgba(214, 51, 108, 0.2);
      margin-bottom: 40px;
      overflow: hidden;
    }
    .product img {
      width: 100%;
      object-fit: cover;
      max-height: 400px;
    }
    .product-info {
      padding: 20px;
    }
    .product-info h2 {
      color: #d6336c;
      margin-bottom: 10px;
    }
    .product-info p {
      font-size: 1.1em;
      margin-bottom: 20px;
    }
    .buttons a {
      display: inline-block;
      background: #d6336c;
      color: white;
      text-decoration: none;
      padding: 12px 20px;
      border-radius: 8px;
      margin-right: 10px;
      font-weight: bold;
      transition: background 0.3s ease;
    }
    .buttons a:hover {
      background: #a5003b;
    }
    footer {
      text-align: center;
      color: #d6336c;
      padding: 30px 0;
      font-weight: 600;
    }
  </style>
</head>
<body>

<header>
  Mi Tienda de Cosmética
</header>

<section id="catalogo">
  <!-- Aquí se cargan los productos -->
</section>

<footer>
  &copy; 2025 Cosmética y Belleza | WhatsApp: +34 624 387 627
</footer>

<script>
  const productos = [
    {
      nombre: "Perfume Elegante de Mujer",
      descripcion: "Aroma floral duradero. Perfecto para cualquier ocasión.",
      imagen: "https://ae01.alicdn.com/kf/S9121738e0a6e42aa8917e61f398b0d8c3.jpg",
      whatsapp: "https://wa.me/34624387627?text=Hola,%20quiero%20el%20Perfume%20Elegante"
    },
    {
      nombre: "Paleta Profesional de Sombras",
      descripcion: "Colores intensos y duraderos para maquillaje profesional.",
      imagen: "https://ae01.alicdn.com/kf/Sb04d2c97c2b94c51a15cfdb4db048c0fj.jpg",
      whatsapp: "https://wa.me/34624387627?text=Hola,%20quiero%20la%20paleta%20de%20sombras"
    },
    {
      nombre: "Base de Maquillaje Matte",
      descripcion: "Acabado suave y natural. Ideal para el uso diario.",
      imagen: "https://ae01.alicdn.com/kf/S2e8c8c3c7415439a9a2e2f72a290a0f7l.jpg",
      whatsapp: "https://wa.me/34624387627?text=Hola,%20quiero%20la%20base%20de%20maquillaje"
    }
  ];

  const contenedor = document.getElementById('catalogo');
  productos.forEach(p => {
    const card = document.createElement('div');
    card.className = 'product';
    card.innerHTML = `
      <img src="${p.imagen}" alt="${p.nombre}">
      <div class="product-info">
        <h2>${p.nombre}</h2>
        <p>${p.descripcion}</p>
        <div class="buttons">
          <a href="${p.whatsapp}" target="_blank">Encargar por WhatsApp</a>
        </div>
      </div>
    `;
    contenedor.appendChild(card);
  });
</script>

</body>
</html>
