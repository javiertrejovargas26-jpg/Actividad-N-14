# Actividad-N-14
actividad
html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Segoe UI', Roboto, sans-serif;
  color: #333;
  overflow-x: hidden;
}

.bg-custom {
  background-color: #004d40;
}

.text-custom {
  color: #004d40;
}

/* ===== HERO SECTION ===== */
.hero {
  height: 100vh;
  background: linear-gradient(135deg, #004d40, #00796b);
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  text-shadow: 0 2px 5px rgba(0,0,0,0.3);
  animation: fadeIn 2s ease;
}

/* ===== BOTONES PERSONALIZADOS ===== */
.btn-custom {
  background-color: #ffffff;
  color: #004d40;
  border-radius: 50px;
  font-weight: 600;
  transition: all 0.3s ease;
}

.btn-custom:hover {
  background-color: #00796b;
  color: #fff;
  transform: translateY(-2px);
}

/* ===== CARDS DE CLIENTES ===== */
.card {
  border-radius: 15px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

/* ===== FOOTER ===== */
footer {
  font-size: 0.9rem;
  letter-spacing: 0.5px;
}

/* ===== ANIMACIONES ===== */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}

.animate-fade {
  animation: fadeIn 1.5s ease;
}

/* ===== FORM VALIDATION ===== */
.was-validated .form-control:invalid {
  border-color: #dc3545;
  background-image: none;
}

.was-validated .form-control:valid {
  border-color: #004d40;
}

.form-control:focus {
  box-shadow: 0 0 5px rgba(0,77,64,0.5);
  border-color: #004d40;
}
<!DOCTYPE html>
<html lang="es">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>NovaTech Pro - Transformación Digital</title>

  <!-- Bootstrap 5 (CDN) -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>

  <!-- Bootstrap Icons CDN -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">

  <!-- CSS personalizado -->
  <link rel="stylesheet" href="css/style.css">
</head>

<body>

  <!-- ================= Header con Navbar ================= -->
  <header>
    <nav class="navbar navbar-expand-lg navbar-dark bg-custom fixed-top shadow-sm">
      <div class="container">
        <a class="navbar-brand" href="#">NovaTech Pro</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item"><a class="nav-link" href="#inicio">Inicio</a></li>
            <li class="nav-item"><a class="nav-link" href="#soluciones">Soluciones</a></li>
            <li class="nav-item"><a class="nav-link" href="#clientes">Clientes</a></li>
            <li class="nav-item"><a class="nav-link" href="#contacto">Contáctanos</a></li>
          </ul>
        </div>
      </div>
    </nav>
  </header>

  <!-- ================= Main (contenido principal) ================= -->
  <main>
    <!-- Sección Hero -->
    <section id="inicio" class="hero bg-custom text-white text-center p-5">
      <div class="container">
        <h1 class="display-3 fw-bold">Transforma tu negocio con NovaTech Pro</h1>
        <p class="lead">Soluciones digitales innovadoras que impulsan tu empresa hacia el futuro.</p>
        <a href="#soluciones" class="btn btn-custom btn-lg mt-3">Descubre nuestras soluciones</a>
      </div>
    </section>

    <!-- Sección de Soluciones -->
    <section id="soluciones" class="py-5">
      <div class="container">
        <h2 class="text-center mb-4">Nuestras Soluciones</h2>

        <!-- Solución 1: Consultoría Estratégica -->
        <div class="row align-items-center mb-5">
          <div class="col-md-6 order-md-1">
            <h3>Consultoría Estratégica</h3>
            <p>Impulsamos tu empresa con asesoría estratégica para una transformación digital efectiva.</p>
          </div>
          <div class="col-md-6 order-md-2">
            <img src="https://via.placeholder.com/500x300" alt="Consultoría Estratégica" class="img-fluid rounded-3 shadow-sm">
          </div>
        </div>

        <!-- Solución 2: Desarrollo a Medida -->
        <div class="row align-items-center mb-5">
          <div class="col-md-6">
            <h3>Desarrollo a Medida</h3>
            <p>Creamos soluciones digitales personalizadas para satisfacer las necesidades específicas de tu negocio.</p>
          </div>
          <div class="col-md-6">
            <img src="https://via.placeholder.com/500x300" alt="Desarrollo a Medida" class="img-fluid rounded-3 shadow-sm">
          </div>
        </div>

        <!-- Solución 3: Crecimiento Digital -->
        <div class="row align-items-center">
          <div class="col-md-6 order-md-1">
            <h3>Crecimiento Digital</h3>
            <p>Aumenta tu presencia online y optimiza tus estrategias de marketing digital para captar más clientes.</p>
          </div>
          <div class="col-md-6 order-md-2">
            <img src="https://via.placeholder.com/500x300" alt="Crecimiento Digital" class="img-fluid rounded-3 shadow-sm">
          </div>
        </div>
      </div>
    </section>

    <!-- Sección de Clientes -->
    <section id="clientes" class="bg-light py-5">
      <div class="container">
        <h2 class="text-center mb-4">Clientes Satisfechos</h2>
        <div class="row text-center">
          <div class="col-md-4 mb-4">
            <div class="card shadow-lg">
              <div class="card-body">
                <i class="bi bi-people-fill fs-1 text-custom mb-3"></i>
                <h5>Empresa A</h5>
                <p>"Gracias a NovaTech Pro, nuestra transformación digital fue un éxito rotundo."</p>
              </div>
            </div>
          </div>
          <div class="col-md-4 mb-4">
            <div class="card shadow-lg">
              <div class="card-body">
                <i class="bi bi-briefcase-fill fs-1 text-custom mb-3"></i>
                <h5>Empresa B</h5>
                <p>"El desarrollo a medida de soluciones tecnológicas ha optimizado nuestros procesos."</p>
              </div>
            </div>
          </div>
          <div class="col-md-4 mb-4">
            <div class="card shadow-lg">
              <div class="card-body">
                <i class="bi bi-chat-square-dots-fill fs-1 text-custom mb-3"></i>
                <h5>Empresa C</h5>
                <p>"El soporte continuo nos ha permitido estar siempre a la vanguardia tecnológica."</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Sección de Contacto -->
    <section id="contacto" class="py-5">
      <div class="container">
        <h2 class="text-center mb-4">Contáctanos</h2>
        <form class="col-md-6 offset-md-3">
          <div class="mb-3">
            <label for="nombre" class="form-label">Nombre</label>
            <input type="text" class="form-control" id="nombre" required>
          </div>
          <div class="mb-3">
            <label for="correo" class="form-label">Correo electrónico</label>
            <input type="email" class="form-control" id="correo" required>
          </div>
          <div class="mb-3">
            <label for="mensaje" class="form-label">Mensaje</label>
            <textarea class="form-control" id="mensaje" rows="4" required></textarea>
          </div>
          <div class="text-center">
            <button type="submit" class="btn btn-custom">Enviar</button>
          </div>
        </form>
      </div>
    </section>
  </main>

  <!-- ================= Footer ================= -->
  <footer class="bg-custom text-white text-center py-3">
    <p class="mb-0">© 2025 NovaTech Pro. Todos los derechos reservados.</p>
  </footer>

</body>

</html>
