☕ Café Santander — FASE I
https://img.shields.io/badge/React-19.0+-blue
https://img.shields.io/badge/TypeScript-5.5+-3178C6
https://img.shields.io/badge/Vite-5.4+-646CFF
https://img.shields.io/badge/Node.js-20.0+-brightgreen
https://img.shields.io/badge/Bootstrap-5.3+-purple
https://img.shields.io/badge/License-MIT-yellow


 Tabla de contenidos
Resumen ejecutivo

Integrantes y roles

Objetivos específicos

Características principales

Tecnologías utilizadas

Requisitos previos

Instalación y ejecución

Estructura del proyecto

Mecanismo de login

Formularios y componentes

Rueda catadora digital

Principios de diseño

Logros y alcance

Capturas y demostración

Empaquetado y entrega

Roadmap

Contribución

Contacto

  Resumen ejecutivo
Café Santander es una aplicación front-end que presenta la identidad y el catálogo de Café Santander. La FASE I incluye una interfaz responsiva, navegación con rutas públicas y privadas, formularios, componentes multimedia y un prototipo interactivo de rueda catadora. El objetivo fue entregar una aplicación clara, documentada y lista para ser revisada.

 Integrantes y roles
César Daniel Ávila Barbosa (Líder) — 25% (coordinación y frontend)

Juan David Neira Meza — 25% (componentes y estilos)

Nancy Liliana Sáenz Moreno — 25% (multimedia y pruebas)

Carlos David Pimienta Rivera — 25% (routing y hooks)


 
 Objetivos específicos
Analizar el contexto del comercio electrónico del café y documentar oportunidades

Diseñar un flujo de exploración y compra accesible

Construir una interfaz intuitiva y responsiva

Implementar sistema de autenticación simulado

Desarrollar prototipo de rueda catadora digital

Integrar contenido auténtico sobre tradición cafetera

Aplicar principios de accesibilidad y usabilidad


 Características principales
Diseño responsivo (móvil / tablet / desktop)

Portada con títulos, logo y barra de menú fija

Menú con dropdowns y navegación clara

Rutas públicas y privadas con protección de acceso

Modal de login con credenciales de prueba

Carrito simulado y vista de productos

Formularios con validación básica

Componentes interactivos (modales, collapse, popovers, etc.)

Multimedia integrada (imágenes, audio, video)

Footer con información del equipo


 
 Tecnologías utilizadas
React (v19)

TypeScript (v5.5+)

Vite (v5.4+)

React Router (v7)

Bootstrap 5 + React-Bootstrap

Node.js (v20+)

NOTA: Se eligió TypeScript por ofrecer tipado estático, detección temprana de errores y mayor escalabilidad.

  Requisitos previos
Node.js v18+

npm v9+

Git

Navegador moderno

💻 Instalación y ejecución
Ejecuta los siguientes comandos en PowerShell:

powershell
# 1. Clonar el repositorio y entrar a la carpeta
git clone https://github.com/<usuario>/<repositorio>.git
cd 02_CafeSantander\cafe-react

# 2. Instalar dependencias
npm install

# 3. Ejecutar modo desarrollo
npm run dev

# 4. Para producción
npm run build
npm run preview
Después de npm run dev, abre la URL que Vite indique (ej: http://localhost:5173).

📁 Estructura del proyecto
text
02_CafeSantander/
└─ cafe-react/
   ├─ public/
   │  ├─ imagenes/
   │  ├─ audio/
   │  └─ video/
   ├─ src/
   │  ├─ assets/
   │  ├─ components/
   │  ├─ context/
   │  ├─ hooks/
   │  ├─ pages/
   │  ├─ styles/
   │  ├─ App.tsx
   │  └─ main.tsx
   ├─ package.json
   └─ tsconfig.json
Descripción de carpetas clave:

public/: recursos estáticos (imágenes, audio, video)

src/components/: componentes reutilizables

src/pages/: vistas/rutas de la aplicación

src/context/: contextos React (AuthContext)

src/hooks/: hooks personalizados

src/styles/: archivos CSS organizados

 Mecanismo de login
Modal de login: src/components/BootstrapLoginModal.tsx

Contexto de autenticación: src/context/AuthContext.tsx

Protección de rutas: src/components/PrivateRoute.tsx

Credenciales de evaluación:

Usuario: Admin

Contraseña: 1234

 Formularios y componentes
Formulario de contacto con validación básica

Componentes interactivos: Carrusel, Acordeón, Collapse, Popover, Dropdown

Multimedia con controles de reproducción

Prototipo de rueda catadora en la sección de Productos/Servicios

 Rueda catadora digital
Prototipo interactivo para orientar la selección de café según preferencias sensoriales (sabor, aroma, intensidad). Sirve como base para futuras mejoras.

 Principios de diseño
Contraste de color para legibilidad

Jerarquía visual con tipografías y espaciado

Consistencia visual con componentes reutilizables

Accesibilidad básica: alt en imágenes, labels en formularios

Usabilidad: barra de navegación fija y estructura clara

 Logros y alcance
Interfaz responsiva y navegable

Rutas públicas/privadas con autenticación simulada

Formularios y validaciones implementadas

Componentes interactivos y multimedia integrados

Prototipo de rueda catadora digital

Documentación completa incluida

📸 Capturas y demostración
https:///imagenes/cafe/portada-1.png
https:///imagenes/cafe/login-modal.png
https:///imagenes/cafe/ruleta-catadora.png
https:///imagenes/cafe/historia.png
https:///imagenes/cafe/productos.png

Las imágenes deben estar en public/imagenes/cafe/ para visualizarse correctamente.

 Empaquetado y entrega
Ejecutar npm run build para generar dist/

Crear carpeta 02_App con:

Carpeta cafe-react completa (sin node_modules)

Archivo 02_aplicativo.pdf con documentación

Readme.txt resumido

Comprimir en 02_App.zip y entregar

 Roadmap
Integrar backend para autenticación real

Añadir encuesta y estadísticas

Mejorar rueda catadora con datos guardados

Implementar captcha y validaciones robustas

 Contribución
Fork del proyecto

Crear rama feature: git checkout -b feature/nuevaFuncionalidad

Commit cambios: git commit -m 'feat: nueva funcionalidad'

Push: git push origin feature/nuevaFuncionalidad

Abrir Pull Request

 Contacto
César Daniel Ávila Barbosa — cesar2224642@correo.uis.edu.co

Juan David Neira Meza — cesar2224642@correo.uis.edu.co

Nancy Liliana Sáenz Moreno — nancy2224510@correo.uis.edu.co

Carlos David Pimienta Rivera — carlos2221873@correo.uis.edu.co

