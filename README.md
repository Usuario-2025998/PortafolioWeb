# PortafolioWeb
Mi portafolio web profesional
https://g.co/gemini/share/393bb4e3eb64
<!DOCTYPE html>
<html lang="es" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jesus Acevedo - Preparador Físico</title>
    <meta name="description" content="Portafolio personal de Jesus Acevedo, preparador físico apasionado por crear rutinas y dar buen servicio al cliente.">
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#0A192F', // Dark Blue (fondo principal)
                        secondary: '#F3F4F6', // Light Gray (fondo de algunas secciones)
                        text: '#D1D5DB', // Lighter Gray (texto general sobre fondos oscuros)
                        heading: '#E0E7FF', // Whiteish blue (títulos)
                        accent: '#34D399', // Vibrant Teal (acentos y botones)
                        accentDark: '#10B981', // Darker Teal (hover de acentos)
                    },
                    fontFamily: {
                        montserrat: ['Montserrat', 'sans-serif'],
                        openSans: ['Open Sans', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    
    <!-- Custom CSS para animaciones y estilos específicos -->
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            color: var(--color-text); /* Fallback */
            background-color: theme('colors.primary');
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
            color: theme('colors.heading');
        }

        /* Estilos para el botón de scroll to top */
        #scrollToTopBtn {
            display: none; /* Oculto por defecto */
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1000;
            background-color: theme('colors.accent');
            color: white;
            padding: 0.75rem 1rem;
            border-radius: 9999px; /* Fully rounded */
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: background-color 0.3s ease;
            cursor: pointer;
        }

        #scrollToTopBtn:hover {
            background-color: theme('colors.accentDark');
        }

        /* Animaciones */
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .fade-in.show {
            opacity: 1;
            transform: translateY(0);
        }

        .skill-bar-fill {
            transition: width 0.8s ease-out;
        }
    </style>
</head>
<body class="bg-primary text-text leading-relaxed">

    <!-- Navegación Fija -->
    <header class="fixed top-0 left-0 right-0 z-50 bg-primary shadow-lg">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <a href="#hero" class="text-heading text-2xl font-bold font-montserrat">Jesus Acevedo</a>
            
            <!-- Botón Hamburguesa para móvil -->
            <button id="menu-toggle" class="md:hidden text-heading focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
                </svg>
            </button>

            <!-- Menú de Navegación -->
            <ul id="main-nav" class="hidden md:flex space-x-8">
                <li><a href="#hero" class="nav-link text-text hover:text-accent transition duration-300 active-link">Inicio</a></li>
                <li><a href="#about" class="nav-link text-text hover:text-accent transition duration-300">Sobre Mí</a></li>
                <li><a href="#skills" class="nav-link text-text hover:text-accent transition duration-300">Habilidades</a></li>
                <li><a href="#experience" class="nav-link text-text hover:text-accent transition duration-300">Experiencia</a></li>
                <li><a href="#education" class="nav-link text-text hover:text-accent transition duration-300">Educación</a></li>
                <li><a href="#portfolio" class="nav-link text-text hover:text-accent transition duration-300">Proyectos</a></li>
                <li><a href="#contact" class="nav-link text-text hover:text-accent transition duration-300">Contacto</a></li>
            </ul>
        </nav>

        <!-- Menú Móvil Desplegable -->
        <ul id="mobile-nav" class="md:hidden hidden bg-primary shadow-lg py-2">
            <li><a href="#hero" class="block px-4 py-2 text-text hover:bg-accent hover:text-primary transition duration-300">Inicio</a></li>
            <li><a href="#about" class="block px-4 py-2 text-text hover:bg-accent hover:text-primary transition duration-300">Sobre Mí</a></li>
            <li><a href="#skills" class="block px-4 py-2 text-text hover:bg-accent hover:text-primary transition duration-300">Habilidades</a></li>
            <li><a href="#experience" class="block px-4 py-2 text-text hover:bg-accent hover:text-primary transition duration-300">Experiencia</a></li>
            <li><a href="#education" class="block px-4 py-2 text-text hover:bg-accent hover:text-primary transition duration-300">Educación</a></li>
            <li><a href="#portfolio" class="block px-4 py-2 text-text hover:bg-accent hover:text-primary transition duration-300">Proyectos</a></li>
            <li><a href="#contact" class="block px-4 py-2 text-text hover:bg-accent hover:text-primary transition duration-300">Contacto</a></li>
        </ul>
    </header>

    <main>
        <!-- 1. Sección de Inicio (Hero Section) -->
        <section id="hero" class="relative min-h-screen flex items-center justify-center text-center bg-cover bg-center" style="background-image: url('https://placehold.co/1920x1080/0A192F/E0E7FF?text=Profesionalismo+Deportivo');">
            <!-- Capa de superposición para mejor contraste -->
            <div class="absolute inset-0 bg-primary opacity-80"></div>
            
            <div class="relative z-10 max-w-4xl px-4 sm:px-6 lg:px-8 fade-in">
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-heading mb-4 font-montserrat leading-tight">
                    Profesionalismo en Deportes
                </h1>
                <p class="text-2xl sm:text-3xl text-text font-semibold font-montserrat mb-2">
                    JESUS ACEVEDO
                </p>
                <p class="text-xl sm:text-2xl text-accent font-medium font-montserrat mb-6">
                    Preparador Físico
                </p>
                <p class="text-lg sm:text-xl text-text max-w-2xl mx-auto mb-10 font-openSans">
                    Apasionado por crear rutinas y dar buen servicio al cliente en mi área deportiva como entrenador de gym.
                </p>
                <div class="flex flex-col sm:flex-row justify-center gap-4">
                    <a href="#portfolio" class="btn bg-accent text-primary px-8 py-3 rounded-full text-lg font-semibold hover:bg-accentDark transition duration-300 transform hover:scale-105 shadow-lg">
                        Ver Mis Proyectos
                    </a>
                    <a href="#" class="btn bg-transparent border-2 border-accent text-accent px-8 py-3 rounded-full text-lg font-semibold hover:bg-accent hover:text-primary transition duration-300 transform hover:scale-105 shadow-lg">
                        Descargar CV
                    </a>
                </div>
            </div>
        </section>

        <!-- 2. Sección Acerca de Mí (About Me) -->
        <section id="about" class="py-16 sm:py-20 lg:py-24 bg-secondary-light fade-in">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-4xl font-bold mb-12 text-heading font-montserrat">Sobre Mí</h2>
                <div class="flex flex-col md:flex-row items-center gap-12">
                    <div class="md:w-1/3 flex justify-center">
                        <img src="https://placehold.co/400x400/0A192F/E0E7FF?text=Mi+Foto" alt="Mi Foto Profesional" class="rounded-full w-64 h-64 object-cover border-4 border-accent shadow-xl transform transition duration-500 hover:scale-105">
                    </div>
                    <div class="md:w-2/3 text-left">
                        <p class="mb-4 text-text font-openSans text-lg">
                            Desde mis inicios en el mundo del entrenamiento, he sido un preparador físico comprometido con el bienestar y los objetivos de mis clientes. Mi experiencia me ha permitido desarrollar una capacidad excepcional para adaptarme a diversas situaciones, especialmente aquellas que requieren un enfoque cuidadoso y personalizado.
                        </p>
                        <p class="mb-4 text-text font-openSans text-lg">
                            Mi trayectoria incluye el manejo exitoso de personas con problemas articulares, donde he aplicado metodologías de entrenamiento seguras y efectivas, logrando mejoras significativas en su movilidad y calidad de vida. La clave ha sido siempre una escucha activa y una planificación meticulosa.
                        </p>
                        <p class="mb-4 text-text font-openSans text-lg">
                            Soy una persona altamente responsable y proactiva, siempre buscando motivar a mis alumnos a superar sus límites de forma segura y consistente. Mi enfoque se centra en crear un ambiente de apoyo y confianza, donde cada persona se sienta empoderada para alcanzar su máximo potencial.
                        </p>
                        <p class="mb-4 text-text font-openSans text-lg">
                            Creo firmemente que la disciplina y la pasión son fundamentales para el éxito, y me esfuerzo por inculcar estos valores en cada sesión. Mi objetivo es no solo transformar cuerpos, sino también fortalecer mentes y espíritus, construyendo hábitos saludables y duraderos.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- 3. Sección Habilidades (Skills) -->
        <section id="skills" class="py-16 sm:py-20 lg:py-24 bg-primary fade-in">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-4xl font-bold mb-12 text-heading font-montserrat">Mis Habilidades</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-3 gap-12 text-left">
                    <!-- Habilidades Técnicas -->
                    <div class="bg-primary-light p-8 rounded-lg shadow-xl border border-gray-700 transform transition duration-500 hover:scale-105">
                        <h3 class="text-2xl font-semibold mb-6 text-accent font-montserrat">Habilidades Técnicas</h3>
                        <ul class="space-y-4 text-text font-openSans">
                            <li>
                                <div class="flex justify-between items-center mb-1">
                                    <span>Planes de Entrenamientos</span>
                                    <span class="text-sm text-heading">Avanzado</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2">
                                    <div class="bg-accent h-2 rounded-full skill-bar-fill" style="width: 95%;"></div>
                                </div>
                            </li>
                            <li>
                                <div class="flex justify-between items-center mb-1">
                                    <span>Diseño de Rutinas</span>
                                    <span class="text-sm text-heading">Avanzado</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2">
                                    <div class="bg-accent h-2 rounded-full skill-bar-fill" style="width: 90%;"></div>
                                </div>
                            </li>
                            <li>
                                <div class="flex justify-between items-center mb-1">
                                    <span>Ejercicios y Sesiones</span>
                                    <span class="text-sm text-heading">Avanzado</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2">
                                    <div class="bg-accent h-2 rounded-full skill-bar-fill" style="width: 90%;"></div>
                                </div>
                            </li>
                        </ul>
                    </div>

                    <!-- Herramientas -->
                    <div class="bg-primary-light p-8 rounded-lg shadow-xl border border-gray-700 transform transition duration-500 hover:scale-105">
                        <h3 class="text-2xl font-semibold mb-6 text-accent font-montserrat">Herramientas</h3>
                        <ul class="space-y-4 text-text font-openSans">
                            <li>
                                <div class="flex justify-between items-center mb-1">
                                    <span>VS Code</span>
                                    <span class="text-sm text-heading">Intermedio</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2">
                                    <div class="bg-accent h-2 rounded-full skill-bar-fill" style="width: 70%;"></div>
                                </div>
                            </li>
                            <li>
                                <div class="flex justify-between items-center mb-1">
                                    <span>Figma</span>
                                    <span class="text-sm text-heading">Básico</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2">
                                    <div class="bg-accent h-2 rounded-full skill-bar-fill" style="width: 40%;"></div>
                                </div>
                            </li>
                            <li>
                                <div class="flex justify-between items-center mb-1">
                                    <span>Adobe XD</span>
                                    <span class="text-sm text-heading">Básico</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2">
                                    <div class="bg-accent h-2 rounded-full skill-bar-fill" style="width: 30%;"></div>
                                </div>
                            </li>
                            <li>
                                <div class="flex justify-between items-center mb-1">
                                    <span>Jira</span>
                                    <span class="text-sm text-heading">Básico</span>
                                </div>
                                <div class="w-full bg-gray-700 rounded-full h-2">
                                    <div class="bg-accent h-2 rounded-full skill-bar-fill" style="width: 50%;"></div>
                                </div>
                            </li>
                        </ul>
                    </div>

                    <!-- Habilidades Blandas -->
                    <div class="bg-primary-light p-8 rounded-lg shadow-xl border border-gray-700 transform transition duration-500 hover:scale-105">
                        <h3 class="text-2xl font-semibold mb-6 text-accent font-montserrat">Habilidades Blandas</h3>
                        <ul class="space-y-4 text-text font-openSans">
                            <li>Comunicación efectiva</li>
                            <li>Trabajo en equipo</li>
                            <li>Resolución de problemas complejos</li>
                            <li>Liderazgo</li>
                            <li>Adaptabilidad</li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- 4. Sección Experiencia Profesional (Experience) -->
        <section id="experience" class="py-16 sm:py-20 lg:py-24 bg-secondary-light fade-in">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-4xl font-bold mb-12 text-heading font-montserrat">Experiencia Laboral</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-left">
                    <!-- Puesto 1 -->
                    <div class="bg-primary p-8 rounded-lg shadow-xl border border-gray-700 transform transition duration-500 hover:scale-105">
                        <h3 class="text-2xl font-semibold text-accent font-montserrat">Entrenador de Planta</h3>
                        <p class="text-lg text-heading font-medium mb-2">Bodytech</p>
                        <p class="text-sm text-gray-400 mb-4">20 de abril del 2025 – 20 de octubre 2025</p>
                        <ul class="list-disc list-inside space-y-2 text-text font-openSans">
                            <li>Logré buenos cambios físicos en los estudiantes a través de programas personalizados.</li>
                            <li>Contribuciones significativas a la mejora cardiovascular de los clientes.</li>
                            <li>Implementación de técnicas para mejorar la resistencia y el rendimiento deportivo.</li>
                            <li>Asesoramiento y seguimiento constante para asegurar la progresión y seguridad en el entrenamiento.</li>
                        </ul>
                    </div>
                    <!-- Puedes añadir más experiencias aquí si lo deseas -->
                </div>
            </div>
        </section>

        <!-- 5. Sección Educación (Education) -->
        <section id="education" class="py-16 sm:py-20 lg:py-24 bg-primary fade-in">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-4xl font-bold mb-12 text-heading font-montserrat">Formación Académica</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-left">
                    <!-- Título 1 -->
                    <div class="bg-primary-light p-8 rounded-lg shadow-xl border border-gray-700 transform transition duration-500 hover:scale-105">
                        <h3 class="text-2xl font-semibold text-accent font-montserrat">Entrenador de Planta</h3>
                        <p class="text-lg text-heading font-medium mb-2">Politécnico Superior</p>
                        <p class="text-sm text-gray-400 mb-4">1 abril 2022 – 16 junio 2025</p>
                        <p class="text-text font-openSans">
                            Formación integral en ciencias del deporte, anatomía, fisiología del ejercicio y metodología del entrenamiento, preparándome para diseñar y supervisar programas de acondicionamiento físico.
                        </p>
                    </div>
                    <!-- Puedes añadir más títulos/certificaciones aquí -->
                </div>
            </div>
        </section>

        <!-- 6. Sección Proyectos Destacados (Portfolio) -->
        <section id="portfolio" class="py-16 sm:py-20 lg:py-24 bg-secondary-light fade-in">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-4xl font-bold mb-12 text-heading font-montserrat">Mis Proyectos</h2>
                
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Proyecto 1 -->
                    <div class="bg-primary rounded-lg shadow-xl border border-gray-700 overflow-hidden transform transition duration-500 hover:scale-105">
                        <img src="https://placehold.co/600x400/0A192F/E0E7FF?text=Proyecto+1" alt="Imagen del Proyecto 1" class="w-full h-48 object-cover">
                        <div class="p-6">
                            <h3 class="text-2xl font-semibold mb-2 text-heading font-montserrat">Plataforma de E-commerce</h3>
                            <p class="text-text font-openSans mb-4 text-md">
                                Plataforma de e-commerce desarrollada para XYZ, donde implementé el carrito de compras y la pasarela de pagos. Enfocado en la experiencia de usuario y la seguridad transaccional.
                            </p>
                            <p class="text-sm text-gray-400 mb-4 font-openSans">
                                Tecnologías: <span class="font-semibold text-accent">React, Node.js, Express, MongoDB</span>
                            </p>
                            <div class="flex justify-center gap-4">
                                <a href="#" class="btn bg-accent text-primary px-4 py-2 rounded-full text-sm font-semibold hover:bg-accentDark transition duration-300">Ver Proyecto</a>
                                <a href="https://github.com/Usuario-2025998/PortafolioWeb" target="_blank" class="btn bg-transparent border-2 border-accent text-accent px-4 py-2 rounded-full text-sm font-semibold hover:bg-accent hover:text-primary transition duration-300">Ver Código</a>
                            </div>
                        </div>
                    </div>

                    <!-- Proyecto 2 -->
                    <div class="bg-primary rounded-lg shadow-xl border border-gray-700 overflow-hidden transform transition duration-500 hover:scale-105">
                        <img src="https://placehold.co/600x400/0A192F/E0E7FF?text=Proyecto+2" alt="Imagen del Proyecto 2" class="w-full h-48 object-cover">
                        <div class="p-6">
                            <h3 class="text-2xl font-semibold mb-2 text-heading font-montserrat">Aplicación Móvil de Fitness</h3>
                            <p class="text-text font-openSans mb-4 text-md">
                                Aplicación para dispositivos móviles que permite a los usuarios seguir rutinas de ejercicio personalizadas y monitorear su progreso diario.
                            </p>
                            <p class="text-sm text-gray-400 mb-4 font-openSans">
                                Tecnologías: <span class="font-semibold text-accent">React Native, Firebase, Redux</span>
                            </p>
                            <div class="flex justify-center gap-4">
                                <a href="#" class="btn bg-accent text-primary px-4 py-2 rounded-full text-sm font-semibold hover:bg-accentDark transition duration-300">Ver Proyecto</a>
                                <a href="https://github.com/Usuario-2025998/PortafolioWeb" target="_blank" class="btn bg-transparent border-2 border-accent text-accent px-4 py-2 rounded-full text-sm font-semibold hover:bg-accent hover:text-primary transition duration-300">Ver Código</a>
                            </div>
                        </div>
                    </div>

                    <!-- Proyecto 3 -->
                    <div class="bg-primary rounded-lg shadow-xl border border-gray-700 overflow-hidden transform transition duration-500 hover:scale-105">
                        <img src="https://placehold.co/600x400/0A192F/E0E7FF?text=Proyecto+3" alt="Imagen del Proyecto 3" class="w-full h-48 object-cover">
                        <div class="p-6">
                            <h3 class="text-2xl font-semibold mb-2 text-heading font-montserrat">Sistema de Gestión de Clientes</h3>
                            <p class="text-text font-openSans mb-4 text-md">
                                Herramienta web para gestionar información de clientes, historial de sesiones y pagos, optimizando la administración de un gimnasio.
                            </p>
                            <p class="text-sm text-gray-400 mb-4 font-openSans">
                                Tecnologías: <span class="font-semibold text-accent">Python, Django, PostgreSQL</span>
                            </p>
                            <div class="flex justify-center gap-4">
                                <a href="#" class="btn bg-accent text-primary px-4 py-2 rounded-full text-sm font-semibold hover:bg-accentDark transition duration-300">Ver Proyecto</a>
                                <a href="https://github.com/Usuario-2025998/PortafolioWeb" target="_blank" class="btn bg-transparent border-2 border-accent text-accent px-4 py-2 rounded-full text-sm font-semibold hover:bg-accent hover:text-primary transition duration-300">Ver Código</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 7. Sección Contacto (Contact) -->
        <section id="contact" class="py-16 sm:py-20 lg:py-24 bg-primary fade-in">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-4xl font-bold mb-12 text-heading font-montserrat">Hablemos</h2>
                
                <div class="flex flex-col md:flex-row items-start gap-12 text-left">
                    <div class="md:w-1/2 w-full bg-secondary-light p-8 rounded-lg shadow-xl border border-gray-700">
                        <h3 class="text-2xl font-semibold mb-6 text-accent font-montserrat">Envíame un Mensaje</h3>
                        <form id="contact-form" class="space-y-6">
                            <div>
                                <label for="name" class="block text-text text-sm font-bold mb-2">Nombre</label>
                                <input type="text" id="name" name="name" class="w-full px-4 py-3 rounded-md bg-primary border border-gray-600 text-text focus:outline-none focus:border-accent" placeholder="Tu Nombre" required>
                            </div>
                            <div>
                                <label for="email" class="block text-text text-sm font-bold mb-2">Email</label>
                                <input type="email" id="email" name="email" class="w-full px-4 py-3 rounded-md bg-primary border border-gray-600 text-text focus:outline-none focus:border-accent" placeholder="tu.email@ejemplo.com" required>
                            </div>
                            <div>
                                <label for="subject" class="block text-text text-sm font-bold mb-2">Asunto (Opcional)</label>
                                <input type="text" id="subject" name="subject" class="w-full px-4 py-3 rounded-md bg-primary border border-gray-600 text-text focus:outline-none focus:border-accent" placeholder="Asunto del Mensaje">
                            </div>
                            <div>
                                <label for="message" class="block text-text text-sm font-bold mb-2">Mensaje</label>
                                <textarea id="message" name="message" rows="6" class="w-full px-4 py-3 rounded-md bg-primary border border-gray-600 text-text focus:outline-none focus:border-accent" placeholder="Tu Mensaje..." required></textarea>
                            </div>
                            <button type="submit" class="btn bg-accent text-primary px-8 py-3 rounded-full text-lg font-semibold hover:bg-accentDark transition duration-300 transform hover:scale-105 shadow-lg">
                                Enviar Mensaje
                            </button>
                        </form>
                    </div>

                    <div class="md:w-1/2 w-full bg-secondary-light p-8 rounded-lg shadow-xl border border-gray-700">
                        <h3 class="text-2xl font-semibold mb-6 text-accent font-montserrat">Información de Contacto</h3>
                        <ul class="space-y-6 text-text font-openSans text-lg">
                            <li>
                                <span class="font-bold text-heading">Email:</span> <a href="mailto:gokuyvegeta2045@gmail.com" class="text-accent hover:underline">gokuyvegeta2045@gmail.com</a>
                            </li>
                            <li>
                                <span class="font-bold text-heading">GitHub:</span> <a href="https://github.com/Usuario-2025998/PortafolioWeb" target="_blank" class="text-accent hover:underline">Usuario-2025998/PortafolioWeb</a>
                            </li>
                            <!-- Puedes añadir más información de contacto aquí (ej: LinkedIn, Teléfono) -->
                        </ul>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-primary py-8 text-center text-text text-sm border-t border-gray-700">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            &copy; <span id="current-year"></span> Jesus Acevedo. Todos los derechos reservados.
        </div>
    </footer>

    <!-- Botón de Scroll to Top -->
    <button id="scrollToTopBtn" aria-label="Volver arriba">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 10l7-7m0 0l7 7m-7-7v18" />
        </svg>
    </button>

    <!-- Custom Message Box (instead of alert) -->
    <div id="message-box" class="hidden fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-[9999]">
        <div class="bg-secondary-light p-8 rounded-lg shadow-xl text-center max-w-sm w-full border border-gray-700">
            <h3 id="message-box-title" class="text-2xl font-bold text-heading mb-4 font-montserrat"></h3>
            <p id="message-box-content" class="text-text mb-6 font-openSans"></p>
            <button id="message-box-close" class="btn bg-accent text-primary px-6 py-2 rounded-full text-md font-semibold hover:bg-accentDark transition duration-300">
                Aceptar
            </button>
        </div>
    </div>


    <!-- JavaScript -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Actualizar año en el footer
            document.getElementById('current-year').textContent = new Date().getFullYear();

            // Toggle del menú móvil
            const menuToggle = document.getElementById('menu-toggle');
            const mobileNav = document.getElementById('mobile-nav');
            menuToggle.addEventListener('click', () => {
                mobileNav.classList.toggle('hidden');
            });

            // Smooth scroll para enlaces de navegación
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                    // Ocultar menú móvil después de clickear en un enlace
                    if (!mobileNav.classList.contains('hidden')) {
                        mobileNav.classList.add('hidden');
                    }
                });
            });

            // Resaltar enlace de navegación activo al hacer scroll
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('.nav-link');

            const options = {
                root: null, // viewport
                rootMargin: '0px',
                threshold: 0.5 // Porcentaje de visibilidad para considerar activa la sección
            };

            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        navLinks.forEach(link => {
                            link.classList.remove('active-link');
                            link.classList.remove('text-accent');
                            link.classList.add('text-text'); // Restaurar color por defecto
                        });
                        const correspondingLink = document.querySelector(`.nav-link[href="#${entry.target.id}"]`);
                        if (correspondingLink) {
                            correspondingLink.classList.add('active-link');
                            correspondingLink.classList.remove('text-text'); // Quitar color por defecto
                            correspondingLink.classList.add('text-accent'); // Añadir color de acento
                        }
                    }
                });
            }, options);

            sections.forEach(section => {
                observer.observe(section);
            });

            // Animación fade-in al hacer scroll
            const fadeInElements = document.querySelectorAll('.fade-in');
            const fadeInObserver = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('show');
                        fadeInObserver.unobserve(entry.target); // Dejar de observar una vez que se muestra
                    }
                });
            }, {
                rootMargin: '0px',
                threshold: 0.1 // Mostrar cuando el 10% del elemento es visible
            });

            fadeInElements.forEach(el => {
                fadeInObserver.observe(el);
            });

            // Animación de las barras de habilidad (activar al hacer scroll)
            const skillBars = document.querySelectorAll('.skill-bar-fill');
            const skillObserver = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        // Activar la animación de la barra
                        const width = entry.target.style.width; // Obtener el ancho definido en el estilo inline
                        entry.target.style.width = '0%'; // Resetear a 0 para animar
                        setTimeout(() => {
                            entry.target.style.width = width; // Aplicar el ancho real con transición
                        }, 100); // Pequeño retraso para asegurar el reset

                        skillObserver.unobserve(entry.target); // Dejar de observar
                    }
                });
            }, {
                threshold: 0.5
            });

            skillBars.forEach(bar => {
                skillObserver.observe(bar);
            });

            // Botón de Scroll to Top
            const scrollToTopBtn = document.getElementById('scrollToTopBtn');

            window.addEventListener('scroll', () => {
                if (window.scrollY > 300) { // Mostrar botón después de 300px de scroll
                    scrollToTopBtn.style.display = 'block';
                } else {
                    scrollToTopBtn.style.display = 'none';
                }
            });

            scrollToTopBtn.addEventListener('click', () => {
                window.scrollTo({
                    top: 0,
                    behavior: 'smooth'
                });
            });

            // Manejo del formulario de contacto (simulado)
            const contactForm = document.getElementById('contact-form');
            const messageBox = document.getElementById('message-box');
            const messageBoxTitle = document.getElementById('message-box-title');
            const messageBoxContent = document.getElementById('message-box-content');
            const messageBoxClose = document.getElementById('message-box-close');

            contactForm.addEventListener('submit', function(e) {
                e.preventDefault(); // Prevenir el envío real del formulario

                // Simular envío
                console.log('Formulario enviado:', {
                    name: document.getElementById('name').value,
                    email: document.getElementById('email').value,
                    subject: document.getElementById('subject').value,
                    message: document.getElementById('message').value,
                });

                // Mostrar mensaje de éxito
                messageBoxTitle.textContent = '¡Mensaje Enviado!';
                messageBoxContent.textContent = 'Gracias por contactarme. Me pondré en contacto contigo pronto.';
                messageBox.classList.remove('hidden');

                // Limpiar el formulario
                contactForm.reset();
            });

            messageBoxClose.addEventListener('click', () => {
                messageBox.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
