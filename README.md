# Alerta Vial

Sitio web informativo de un proyecto de ingeniería que propone un sistema de sensor para prevenir accidentes en las intersecciones donde existe una señal de PARE, la cual por confianza o intuision se saltan y ocurren accidentes, principalmente en horas de la noche.
- LINK: [Alerta Vial - Formulacion TIC](https://alertavialtic.netlify.app/)

---

## Descripción del Proyecto

**Alerta Vial** es la plataforma web de divulgación de un proyecto de seguridad vial. El sitio presenta la problemática, la solución propuesta, el funcionamiento conceptual del sistema, el público objetivo y el equipo de ingenieros a cargo.

> **Importante:** este repositorio contiene únicamente el sitio web (landing page) del proyecto. No incluye el firmware, código de sensores ni la lógica de hardware del dispositivo; es la capa de presentación y difusión de la idea.

El sistema propuesto (fuera de este repositorio) detectaría cuando un vehículo se aproxima a una señal de PARE en horas nocturnas y activaría una alerta visual/sonora para reducir accidentes por incumplimiento de la señal.

---

## Problemática

* Conductores que no respetan la señal de PARE, especialmente en la noche
* Alta tasa de accidentes en intersecciones con baja visibilidad
* Falta de control y monitoreo en tiempo real
* Poca cultura de seguridad vial

---

## Solución Propuesta

* Sensor de detección de vehículos en la intersección
* Identificación el flujo de carro en la via contraria a la señal PARE
* Activación de alertas visuales/sonoras de la misma señal de PARE
* Divulgación del proyecto a través de esta plataforma web

---

## Funcionalidades del sitio

* Página principal con carrusel informativo sobre la señal PARE
* Sección "About Us" con la propuesta de valor del proyecto
* Sección "Impacto" explicando cómo funcionaría el sistema y sus beneficios
* Sección "Areas" indicando el público objetivo
* Sección "Engineers" con el equipo del proyecto (carrusel de integrantes)
* Formulario de contacto funcional (envío de correo vía backend en PHP)

---

## Tecnologías Utilizadas

| Tecnología | Uso en el proyecto |
|---|---|
| **HTML5 / CSS3** | Estructura y estilos de las 5 páginas del sitio |
| **SCSS** | Fuente de estilos (`scss/style.scss`), compilada a `css/style.css` |
| **Bootstrap 4** | Sistema de grillas y componentes UI |
| **jQuery 3.4.1** | Manipulación del DOM e interacciones |
| **OwlCarousel 2** | Carruseles de imágenes y del equipo de trabajo |
| **Tempus Dominus** | Selector de fecha/hora en el formulario de contacto |
| **Font Awesome 5** | Iconografía del sitio |
| **Google Fonts** (Montserrat, Roboto) | Tipografía |
| **PHP** | Backend simple (`mail/contact.php`) que procesa y envía el formulario de contacto por correo |

---

## Estructura del Proyecto

```bash
FormulacionTic-AlertaVial
├── index.html          # Página principal (Home)
├── about.html           # Sobre el proyecto (About Us)
├── funtion.html          # Cómo funciona / Impacto y beneficios
├── practice.html         # Público objetivo (Areas)
├── team.html             # Equipo de ingenieros (Engineers)
├── css/
│   ├── style.css
│   └── style.min.css
├── scss/                 # Fuente SCSS (Bootstrap + estilos propios)
├── js/
│   └── main.js           # Carruseles, datetimepicker, scroll-to-top
├── mail/
│   ├── contact.php       # Procesa el envío del formulario de contacto
│   └── contact.js
├── img/                  # Imágenes del sitio (logos, señal PARE, equipo)
└── lib/                  # Librerías de terceros (OwlCarousel, Tempus Dominus, easing, waypoints)
```

---

## Instalación y Despliegue

Al ser un sitio estático (HTML/CSS/JS), puede visualizarse de dos formas:

**1. Localmente (rápido, sin backend):**
```bash
git clone https://github.com/juandiegogalindo/FormulacionTic-AlertaVial.git
cd FormulacionTic-AlertaVial
```
Abrir `index.html` directamente en el navegador. El formulario de contacto **no enviará correos** de esta forma, ya que `contact.php` requiere un servidor con PHP.

**2. Despliegue en producción:**
El proyecto está pensado para desplegarse como sitio estático en un dominio público (por ejemplo Netlify), donde las páginas se sirven directamente sin necesidad de configuración adicional.

---

## Equipo de Ingenieros

| Rol | Integrante |
|---|---|
| Ingeniero Civil | David Munar |
| Ingeniero de Telecomunicaciones | Adriam Angel |
| Ingeniera de Sistemas | Juanita Campos |
| Ingeniero de Sistemas | Santiago Parra |
| Ingeniero de Sistemas | **Juan Diego Galindo** |

---

## Futuras Mejoras

* Integración con app móvil
* Uso de inteligencia artificial para el análisis de patrones de infracción
* Análisis de datos en tiempo real
* Integración con autoridades de tránsito

---

**Juan Diego Galindo**
Estudiante de Ingeniería de Sistemas - Séptimo Semestre
 
- GitHub: [@juandiegogalindo](https://github.com/juandiegogalindo)
- LinkedIn: [Juan Diego Galindo - Full Stack](https://linkedin.com/in/jdgalindo6)
