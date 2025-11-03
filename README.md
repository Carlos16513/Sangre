<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="author" content="Carlos Eduardo Callo Gastañaga">
    <title>SangreSolidaria - Plataforma para Donantes Voluntarios de Sangre</title>
    <!-- Bootstrap CDN para diseño profesional y responsivo -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
    <!-- Estilos personalizados -->
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f8f9fa;
        }
        .hero {
            background-color: #dc3545; /* Rojo sangre para impacto */
            color: white;
            padding: 100px 0;
            text-align: center;
        }
        .hero h1 {
            font-size: 3rem;
            font-weight: bold;
        }
        .section-title {
            font-size: 2rem;
            margin-bottom: 20px;
            color: #dc3545;
        }
        .card {
            border: none;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .form-control:focus {
            border-color: #dc3545;
            box-shadow: 0 0 0 0.25rem rgba(220,53,69,0.25);
        }
        footer {
            background-color: #343a40;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        .alert-example {
            background-color: #fff3cd;
            border: 1px solid #ffeeba;
            padding: 15px;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>

    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-light sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#">SangreSolidaria</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#inicio">Inicio</a></li>
                    <li class="nav-item"><a class="nav-link" href="#registro">Registro</a></li>
                    <li class="nav-item"><a class="nav-link" href="#alertas">Alertas</a></li>
                    <li class="nav-item"><a class="nav-link" href="#campanas">Campañas</a></li>
                    <li class="nav-item"><a class="nav-link" href="#educacion">Educación</a></li>
                    <li class="nav-item"><a class="nav-link" href="#panel">Panel Hospital</a></li>
                    <li class="nav-item"><a class="nav-link" href="#puntos">Puntos</a></li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="inicio" class="hero">
        <div class="container">
            <h1>Únete a SangreSolidaria</h1>
            <p>Facilitamos la donación de sangre para salvar vidas de niños con cáncer en Perú.</p>
            <a href="#registro" class="btn btn-light btn-lg">Regístrate como Donante</a>
        </div>
    </section>

    <!-- Sección de Problemática -->
    <section class="py-5">
        <div class="container">
            <h2 class="section-title text-center">La Problemática en Perú</h2>
            <p class="text-center">Muchos niños con cáncer enfrentan dificultades para acceder a transfusiones de sangre oportunas debido a la escasez de donantes voluntarios, la falta de coordinación entre hospitales y bancos de sangre, y la baja concientización ciudadana.</p>
        </div>
    </section>

    <!-- Sección de Registro de Donantes -->
    <section id="registro" class="bg-light py-5">
        <div class="container">
            <h2 class="section-title text-center">Registro de Donantes Voluntarios</h2>
            <div class="row justify-content-center">
                <div class="col-md-6">
                    <div class="card p-4">
                        <form>
                            <div class="mb-3">
                                <label for="nombre" class="form-label">Nombre</label>
                                <input type="text" class="form-control" id="nombre" placeholder="Ingresa tu nombre">
                            </div>
                            <div class="mb-3">
                                <label for="email" class="form-label">Email</label>
                                <input type="email" class="form-control" id="email" placeholder="Ingresa tu email">
                            </div>
                            <div class="mb-3">
                                <label for="tipoSanguineo" class="form-label">Tipo Sanguíneo</label>
                                <select class="form-select" id="tipoSanguineo">
                                    <option selected>Selecciona...</option>
                                    <option value="A+">A+</option>
                                    <option value="A-">A-</option>
                                    <option value="B+">B+</option>
                                    <option value="B-">B-</option>
                                    <option value="AB+">AB+</option>
                                    <option value="AB-">AB-</option>
                                    <option value="O+">O+</option>
                                    <option value="O-">O-</option>
                                </select>
                            </div>
                            <div class="mb-3">
                                <label for="ubicacion" class="form-label">Ubicación</label>
                                <input type="text" class="form-control" id="ubicacion" placeholder="Ingresa tu ciudad o dirección">
                            </div>
                            <button type="submit" class="btn btn-danger btn-block">Registrarse</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Alertas Geolocalizadas -->
    <section id="alertas" class="py-5">
        <div class="container">
            <h2 class="section-title text-center">Alertas Geolocalizadas</h2>
            <p class="text-center">Recibe notificaciones para donaciones urgentes cerca de ti.</p>
            <div class="alert-example">
                <strong>Alerta Urgente:</strong> Se necesita donante O+ para niño en Hospital Niño Jesús, Lima. ¡Responde ahora!
            </div>
        </div>
    </section>

    <!-- Sección de Agenda de Campañas -->
    <section id="campanas" class="bg-light py-5">
        <div class="container">
            <h2 class="section-title text-center">Agenda de Campañas</h2>
            <div class="row">
                <div class="col-md-4">
                    <div class="card">
                        <div class="card-body">
                            <h5 class="card-title">Campaña en Lima</h5>
                            <p class="card-text">Fecha: 15/11/2025<br>Lugar: Plaza Mayor</p>
                            <a href="#" class="btn btn-danger">Inscribirse</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card">
                        <div class="card-body">
                            <h5 class="card-title">Campaña en Arequipa</h5>
                            <p class="card-text">Fecha: 20/11/2025<br>Lugar: Hospital Regional</p>
                            <a href="#" class="btn btn-danger">Inscribirse</a>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card">
                        <div class="card-body">
                            <h5 class="card-title">Campaña Virtual</h5>
                            <p class="card-text">Fecha: 25/11/2025<br>Lugar: Online</p>
                            <a href="#" class="btn btn-danger">Inscribirse</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Módulo Educativo -->
    <section id="educacion" class="py-5">
        <div class="container">
            <h2 class="section-title text-center">Módulo Educativo</h2>
            <p class="text-center">Aprende sobre el cáncer infantil y la importancia de donar sangre.</p>
            <div class="accordion" id="accordionEducacion">
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingOne">
                        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                            ¿Por qué donar sangre?
                        </button>
                    </h2>
                    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne">
                        <div class="accordion-body">
                            Donar sangre salva vidas, especialmente en casos de niños con cáncer que necesitan transfusiones regulares.
                        </div>
                    </div>
                </div>
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingTwo">
                        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                            Mitos sobre la donación
                        </button>
                    </h2>
                    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo">
                        <div class="accordion-body">
                            Mito: Donar debilita. Realidad: El cuerpo se recupera rápidamente.
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección de Panel de Control para Hospitales -->
    <section id="panel" class="bg-light py-5">
        <div class="container">
            <h2 class="section-title text-center">Panel de Control para Hospitales</h2>
            <p class="text-center">Sigue casos pediátricos y gestiona solicitudes.</p>
            <div class="card p-4">
                <h5>Ejemplo de Dashboard</h5>
                <ul>
                    <li>Casos Pendientes: 5</li>
                    <li>Inventario O+: 10 unidades</li>
                    <li>Donantes Activos: 150</li>
                </ul>
                <a href="#" class="btn btn-danger">Acceder al Panel</a>
            </div>
        </div>
    </section>

    <!-- Sección de Sistema de Puntos -->
    <section id="puntos" class="py-5">
        <div class="container">
            <h2 class="section-title text-center">Sistema de Puntos y Reconocimientos</h2>
            <p class="text-center">Gana puntos por cada donación y obtén badges.</p>
            <div class="row">
                <div class="col-md-4">
                    <div class="card text-center">
                        <div class="card-body">
                            <h1>50</h1>
                            <p>Puntos por donación</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card text-center">
                        <div class="card-body">
                            <h1>Badge Oro</h1>
                            <p>Por 10 donaciones</p>
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card text-center">
                        <div class="card-body">
                            <h1>Ranking</h1>
                            <p>Top donantes</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 SangreSolidaria. Diseñado y desarrollado por Carlos Eduardo Callo Gastañaga.</p>
            <p>Proyecto para Análisis y Diseño de Sistemas de Información I - Escuela Profesional de Ingeniería de Sistemas.</p>
        </div>
    </footer>

    <!-- Bootstrap JS -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js" integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN" crossorigin="anonymous"></script>
</body>
</html>
