<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Tienda Online de Cosmética</title>
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0; padding: 0;
    background: #fff7f8;
    color: #333;
  }
  header {
    background: #f06292;
    color: white;
    padding: 20px;
    text-align: center;
  }
  nav a {
    color: white;
    margin: 0 15px;
    text-decoration: none;
    font-weight: bold;
  }
  .products {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 20px;
    gap: 20px;
  }
  .product-card {
    background: white;
    border-radius: 10px;
    box-shadow: 0 3px 6px #ddd;
    width: 220px;
    padding: 15px;
    text-align: center;
  }
  .product-card img {
    width: 100%;
    border-radius: 10px;
  }
  .product-card h3 {
    margin: 10px 0 5px;
  }
  .product-card p {
    color: #f06292;
    font-weight: bold;
    margin: 5px 0;
  }
  .product-card button {
    background: #f06292;
    border: none;
    color: white;
    padding: 10px;
    border-radius: 5px;
    cursor: pointer;
  }
  footer {
    background: #f06292;
    color: white;
    text-align: center;
    padding: 15px;
    margin-top: 30px;
  }
</style>
</head>
<body>
<header>
  <h1>Tienda de Cosmética</h1>
  <nav>
    <a href="#">Inicio</a>
    <a href="#">Catálogo</a>
    <a href="#">Contacto</a>
  </nav>
</header>

<section class="products">
  <div class="product-card">
    <img src="https://images.unsplash.com/photo-1509475826633-fed577a2c71b?auto=format&fit=crop&w=400&q=80" alt="Labial rojo" />
    <h3>Labial Rojo Intenso</h3>
    <p>$15.99</p>
    <button>Agregar al carrito</button>
  </div>
  <div class="product-card">
    <img src="https://images.unsplash.com/photo-1512418490979-92798cec27d6?auto=format&fit=crop&w=400&q=80" alt="Perfume floral" />
    <h3>Perfume Floral</h3>
    <p>$45.00</p>
    <button>Agregar al carrito</button>
  </div>
  <div class="product-card">
    <img src="https://images.unsplash.com/photo-1542831371-d531d36971e6?auto=format&fit=crop&w=400&q=80" alt="Paleta de sombras" />
    <h3>Paleta de Sombras</h3>
    <p>$22.50</p>
    <button>Agregar al carrito</button>
  </div>
</section>

<footer>
  &copy; 2025 Tienda de Cosmética | Contacto: info@cosmetica.com
</footer>
</body>
</html>
