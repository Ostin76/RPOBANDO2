<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DUALTECH - Tecnología, Ventas y Servicio Técnico</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
        }

        header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            transition: opacity 0.3s;
            font-weight: 500;
        }

        nav a:hover {
            opacity: 0.8;
        }

        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 120px 2rem 80px;
            text-align: center;
            margin-top: 60px;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            animation: fadeInUp 0.8s ease-out;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.95;
            animation: fadeInUp 0.8s ease-out 0.2s backwards;
        }

        .cta-button {
            background: white;
            color: #667eea;
            padding: 1rem 2.5rem;
            border: none;
            border-radius: 50px;
            font-size: 1.1rem;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            font-weight: bold;
            animation: fadeInUp 0.8s ease-out 0.4s backwards;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #333;
        }

        .services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 4rem;
        }

        .service-card {
            background: white;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            text-align: center;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(102,126,234,0.3);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .service-card h3 {
            color: #667eea;
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }

        .products {
            background: #f8f9fa;
            padding: 4rem 2rem;
        }

        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .product-card {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .product-card:hover {
            transform: scale(1.05);
        }

        .product-image {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            height: 200px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4rem;
        }

        .product-info {
            padding: 1.5rem;
        }

        .product-info h3 {
            margin-bottom: 0.5rem;
            color: #333;
        }

        .price {
            color: #667eea;
            font-size: 1.5rem;
            font-weight: bold;
            margin: 1rem 0;
        }

        .contact {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 4rem 2rem;
            text-align: center;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 3rem;
            flex-wrap: wrap;
            margin-top: 2rem;
        }

        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
            font-size: 1.2rem;
        }

        .contact-item span {
            font-size: 2rem;
        }

        footer {
            background: #2d3748;
            color: white;
            text-align: center;
            padding: 2rem;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @media (max-width: 768px) {
            nav ul {
                gap: 1rem;
                font-size: 0.9rem;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1rem;
            }

            .logo {
                font-size: 1.3rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">⚡ DUALTECH</div>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#servicios">Servicios</a></li>
                <li><a href="#productos">Productos</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero" id="inicio">
        <h1>Soluciones Tecnológicas Completas</h1>
        <p>Ventas, Servicio Técnico y Redes - Tu aliado tecnológico de confianza</p>
        <button class="cta-button" onclick="document.getElementById('contacto').scrollIntoView({behavior: 'smooth'})">Contáctanos Ahora</button>
    </section>

    <section class="container" id="servicios">
        <h2 class="section-title">Nuestros Servicios</h2>
        <div class="services">
            <div class="service-card">
                <div class="service-icon">🛠️</div>
                <h3>Servicio Técnico</h3>
                <p>Reparación y mantenimiento de computadoras, laptops y equipos tecnológicos. Diagnóstico rápido y soluciones efectivas.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🌐</div>
                <h3>Instalación de Redes</h3>
                <p>Diseño e implementación de redes cableadas e inalámbricas para hogares y empresas. Configuración profesional.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">💻</div>
                <h3>Venta de Equipos</h3>
                <p>Amplio catálogo de computadoras, laptops, componentes y accesorios tecnológicos de las mejores marcas.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🔒</div>
                <h3>Seguridad Informática</h3>
                <p>Protección de datos, instalación de antivirus, configuración de firewalls y respaldo de información.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">☁️</div>
                <h3>Soluciones en la Nube</h3>
                <p>Migración a la nube, almacenamiento remoto y configuración de servicios cloud para tu negocio.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">📞</div>
                <h3>Soporte Remoto</h3>
                <p>Asistencia técnica a distancia para resolver problemas rápidamente sin necesidad de visitas presenciales.</p>
            </div>
        </div>
    </section>

    <section class="products" id="productos">
        <div class="container">
            <h2 class="section-title">Productos Destacados</h2>
            <div class="product-grid">
                <div class="product-card">
                    <div class="product-image">💻</div>
                    <div class="product-info">
                        <h3>Laptops</h3>
                        <p>Últimos modelos de las mejores marcas</p>
                        <div class="price">Desde $599</div>
                    </div>
                </div>
                <div class="product-card">
                    <div class="product-image">🖥️</div>
                    <div class="product-info">
                        <h3>PCs de Escritorio</h3>
                        <p>Equipos armados a tu medida</p>
                        <div class="price">Desde $499</div>
                    </div>
                </div>
                <div class="product-card">
                    <div class="product-image">🔌</div>
                    <div class="product-info">
                        <h3>Componentes</h3>
                        <p>RAM, discos duros, tarjetas gráficas</p>
                        <div class="price">Varios precios</div>
                    </div>
                </div>
                <div class="product-card">
                    <div class="product-image">📡</div>
                    <div class="product-info">
                        <h3>Equipos de Red</h3>
                        <p>Routers, switches, access points</p>
                        <div class="price">Desde $79</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section class="contact" id="contacto">
        <div class="container">
            <h2 class="section-title" style="color: white;">Contáctanos</h2>
            <p style="font-size: 1.2rem; margin-bottom: 2rem;">Estamos listos para ayudarte con todas tus necesidades tecnológicas</p>
            <div class="contact-info">
                <div class="contact-item">
                    <span>📞</span>
                    <div>
                        <strong>Teléfono</strong><br>
                        +51 999 888 777
                    </div>
                </div>
                <div class="contact-item">
                    <span>📧</span>
                    <div>
                        <strong>Email</strong><br>
                        info@dualtech.com
                    </div>
                </div>
                <div class="contact-item">
                    <span>📍</span>
                    <div>
                        <strong>Dirección</strong><br>
                        Lima, Perú
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 DUALTECH. Todos los derechos reservados. | Soluciones tecnológicas profesionales</p>
    </footer>

    <script>
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
