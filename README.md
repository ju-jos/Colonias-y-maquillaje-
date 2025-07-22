<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Tienda de Cosmética</title>
<style>
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    margin: 0; padding: 0;
    background: #fff0f5;
    color: #333;
  }
  header {
    background: #d6336c;
    color: white;
    padding: 20px;
    text-align: center;
    font-weight: bold;
    font-size: 1.8em;
  }
  nav {
    margin-top: 10px;
  }
  nav a {
    color: white;
    margin: 0 15px;
    text-decoration: none;
    font-weight: 600;
    font-size: 1.1em;
  }
  nav a:hover {
    text-decoration: underline;
  }
  .products {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
    gap: 25px;
    padding: 25px 40px;
  }
  .product-card {
    background: white;
    border-radius: 12px;
    box-shadow: 0 6px 15px rgba(214, 51, 108, 0.3);
    overflow: hidden;
    display: flex;
    flex-direction: column;
    transition: transform 0.2s ease;
  }
  .product-card:hover {
    transform: scale(1.05);
  }
  .product-card img {
    width: 100%;
    object-fit: cover;
    aspect-ratio: 4 / 3;
  }
  .product-info {
    padding: 15px 20px;
    flex-grow: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }
  .product-info h3 {
    margin: 0 0 10px;
    color: #d6336c;
  }
  .product-info p.price {
    font-weight: 700;
    color: #a5003b;
    font-size: 1.2em;
    margin: 0 0 15px;
  }
  .product-info button {
    background: #d6336c;
    border: none;
    color: white;
    padding: 12px 0;
    border-radius: 8px;
    cursor: pointer;
    font-weight: 600;
    font-size: 1em;
    transition: background 0.3s ease;
  }
  .product-info button:hover {
    background: #a5003b;
  }
  footer {
    background: #d6336c;
    color: white;
    text-align: center;
    padding: 15px 0;
    margin-top: 40px;
  }
</style>
</head>
<body>

<header>
  Tienda de Cosmética
  <nav>
    <a href="#">Inicio</a>
    <a href="#">Catálogo</a>
    <a href="#">Contacto</a>
  </nav>
</header>

<section class="products" id="products-container">
  <!-- Los productos se insertan aquí con JavaScript -->
</section>

<footer>
  &copy; 2025 Tienda de Cosmética | Contacto: info@cosmetica.com
</footer>

<script>
  // Aquí defines tus productos
  const productos = [
    {
      nombre: "Labial Rojo Intenso",
      precio: 15.99,
      imagen: "https://images.unsplash.com/photo-1509475826633-fed577a2c71b?auto=format&fit=crop&w=400&q=80",
      descripcion: "Color vibrante y larga duración."
    },
    {
      nombre: "Perfume Floral",
      precio: 45.00,
      imagen: "https://images.unsplash.com/photo-1512418490979-92798cec27d6?auto=format&fit=crop&w=400&q=80",
      descripcion: "Fragancia fresca y elegante."
    },
    {
      nombre: "Paleta de Sombras",
      precio: 22.50,
      imagen: "https://images.unsplash.com/photo-1542831371-d531d36971e6?auto=format&fit=crop&w=400&q=80",
      descripcion: "Colores intensos y variados."
    }
  ];

  const container = document.getElementById('products-container');

  productos.forEach(p => {
    const card = document.createElement('div');
    card.className = 'product-card';

    card.innerHTML = `
      <img src="${p.imagen}" alt="${p.nombre}" />
      <div class="product-info">
        <h3>${p.nombre}</h3>
        <p class="price">$${p.precio.toFixed(2)}</p>
        <p>${p.descripcion}</p>
        <button>Agregar al carrito</button>
      </div>
    `;

    container.appendChild(card);
  });
</script>

</body>
</html>
