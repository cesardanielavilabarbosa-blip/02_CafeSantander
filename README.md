☕ Café Santander — FASE I
https://img.shields.io/badge/React-19.0+-blue
https://img.shields.io/badge/TypeScript-5.5+-3178C6
https://img.shields.io/badge/Vite-5.4+-646CFF
https://img.shields.io/badge/Node.js-20.0+-brightgreen
https://img.shields.io/badge/Bootstrap-5.3+-purple
https://img.shields.io/badge/License-MIT-yellow

📋 Tabla de Contenidos
Instalación y Configuración

Requisitos Previos

Instalación Paso a Paso

Ejecución del Proyecto

Acceso a la Aplicación

Credenciales de Prueba

Solución de Problemas

Tecnologías Utilizadas

Estructura del Proyecto

Características Principales

Equipo de Desarrollo

Contacto de los Integrantes

Valor del Proyecto

🚀 Instalación y Configuración
Requisitos Previos
Antes de comenzar, asegúrate de tener instalado:

Node.js 18.0+ o superior - Descargar

npm 9.0+ o superior (viene con Node.js)

Git - Descargar

Navegador moderno (Chrome, Firefox, Safari, Edge)

Conexión a internet (para descargar dependencias)

Verificación de Requisitos
bash
# Verificar Node.js
node --version

# Verificar npm
npm --version

# Verificar Git
git --version
📥 Instalación Paso a Paso
1. Clonar el Repositorio
bash
# Clonar el repositorio
git clone https://github.com/<usuario>/02_CafeSantander.git

# Navegar al directorio del proyecto
cd 02_CafeSantander/cafe-react
2. Instalar Dependencias
bash
# Instalar todas las dependencias del proyecto
npm install
Dependencias que se instalarán:

React 19.0+

TypeScript 5.5+

Vite 5.4+

React Router DOM 7.0+

Bootstrap 5.3+

React-Bootstrap

3. Verificar Instalación
bash
# Verificar que no hay errores en la instalación
npm run build
🎯 Ejecución del Proyecto
Opción 1: Modo Desarrollo (Recomendado)
bash
# Ejecutar en modo desarrollo
npm run dev
Esto iniciará:

Servidor de desarrollo Vite en http://localhost:5173

Recarga automática en cambios (Hot Reload)

Herramientas de desarrollo React

Opción 2: Modo Producción
bash
# Construir para producción
npm run build

# Previsualizar build de producción
npm run preview
Opción 3: Scripts Disponibles
bash
# Desarrollo
npm run dev

# Producción
npm run build

# Preview producción
npm run preview

# Linter
npm run lint

# Tipo check TypeScript
npm run type-check
🌐 Acceso a la Aplicación
Una vez ejecutado el proyecto:

URLs Principales
Aplicación Web: http://localhost:5173

Página de Inicio: http://localhost:5173/

Productos: http://localhost:5173/productos

Servicios: http://localhost:5173/servicios

Contacto: http://localhost:5173/contacto

Acceso desde Dispositivos Móviles
bash
# En la misma red WiFi, buscar la URL "Network" en la terminal:
  VITE v5.4.11  ready in 256 ms

  ➜  Local:   http://localhost:5173
  ➜  Network: http://192.168.1.XX:5173  # ← Usar esta IP en el celular
🔐 Credenciales de Prueba
Para acceder a las rutas protegidas:

Login de Evaluación
Usuario: Admin

Contraseña: 1234

Rutas Protegidas Accesibles
Carrito de compras

Área de usuario

Historial de pedidos

🐛 Solución de Problemas
Error: "Cannot find module"
bash
# Eliminar node_modules y reinstalar
rm -rf node_modules
rm package-lock.json
npm install
Error: "Port already in use"
bash
# Matar proceso del puerto 5173 (Windows)
npx kill-port 5173

# O usar otro puerto
npm run dev -- --port 3000
Error: TypeScript compilation
bash
# Verificar tipos TypeScript
npm run type-check

# Reinstalar TypeScript
npm install typescript --save-dev
Error: Dependencias faltantes
bash
# Instalar dependencias específicas
npm install react react-dom
npm install @types/react @types/react-dom
npm install react-router-dom
npm install bootstrap react-bootstrap
Problemas de CORS (si se integra con backend)
bash
# Instalar CORS para desarrollo
npm install cors --save-dev
🛠 Tecnologías Utilizadas
Frontend Principal
React 19.0+ - Biblioteca de interfaz de usuario

TypeScript 5.5+ - Superset tipado de JavaScript

Vite 5.4+ - Herramienta de build y desarrollo

React Router DOM 7.0+ - Navegación y rutas

UI y Estilos
Bootstrap 5.3+ - Framework CSS

React-Bootstrap - Componentes Bootstrap para React

CSS3 - Estilos personalizados

Herramientas de Desarrollo
ESLint - Linter para calidad de código

TypeScript Compiler - Verificación de tipos

Git - Control de versiones

📁 Estructura del Proyecto
text
02_CafeSantander/
├── cafe-react/                 # Directorio principal
│   ├── public/                 # Archivos estáticos
│   │   ├── imagenes/           # Logos, fotos del café
│   │   ├── audio/              # Archivos de audio
│   │   └── video/              # Archivos de video
│   ├── src/                    # Código fuente
│   │   ├── components/         # Componentes reutilizables
│   │   │   ├── Header.tsx      # Navegación principal
│   │   │   ├── Footer.tsx      # Pie de página
│   │   │   ├── ProductCard.tsx # Tarjeta de producto
│   │   │   ├── PrivateRoute.tsx # Ruta protegida
│   │   │   └── BootstrapLoginModal.tsx # Modal de login
│   │   ├── pages/              # Páginas/Vistas
│   │   │   ├── Inicio.tsx      # Página principal
│   │   │   ├── Productos.tsx   # Catálogo
│   │   │   ├── Servicios.tsx   # Servicios
│   │   │   ├── Contacto.tsx    # Formulario contacto
│   │   │   └── Carrito.tsx     # Carrito compras
│   │   ├── context/            # Contextos React
│   │   │   └── AuthContext.tsx # Autenticación
│   │   ├── hooks/              # Hooks personalizados
│   │   │   └── useCart.ts      # Gestión carrito
│   │   ├── styles/             # Estilos CSS
│   │   ├── App.tsx             # Componente principal
│   │   └── main.tsx            # Punto de entrada
│   ├── package.json            # Dependencias y scripts
│   ├── tsconfig.json           # Configuración TypeScript
│   └── vite.config.ts          # Configuración Vite
⭐ Características Principales
Funcionalidades Implementadas
✅ Interfaz responsiva (móvil, tablet, desktop)

✅ Sistema de autenticación con rutas protegidas

✅ Catálogo de productos con tarjetas interactivas

✅ Carrito de compras simulado

✅ Formularios de contacto con validación

✅ Rueda catadora digital interactiva

✅ Navegación SPA con React Router

✅ Modales y componentes Bootstrap

Componentes Destacados
Header con navegación responsive

Footer con información del equipo

ProductCard para mostrar productos

BootstrapLoginModal para autenticación

PrivateRoute para protección de rutas

👥 Equipo de Desarrollo
Integrantes y Responsabilidades
Integrante	Rol	Responsabilidad
César Daniel Ávila Barbosa	Líder	Coordinación y Frontend (25%)
Juan David Neira Meza	Desarrollador	Componentes y Estilos (25%)
Nancy Liliana Sáenz Moreno	QA	Multimedia y Pruebas (25%)
Carlos David Pimienta Rivera	Desarrollador	Routing y Hooks (25%)
Curso y Institución
Curso: Diseño de Aplicaciones Web

Docente: Manuel Flórez

Universidad: Universidad Industrial de Santander

Fecha de entrega: 27 de octubre de 2025

📧 Contacto de los Integrantes
César Daniel Ávila Barbosa — cesar2224642@correo.uis.edu.co — 25%

Juan David Neira Meza — juan2235605@correo.uis.edu.co — 25%

Nancy Liliana Sáenz Moreno — nancy2224510@correo.uis.edu.co — 25%

Carlos David Pimienta Rivera — carlos2221873@correo.uis.edu.co — 25%

💡 Valor del Proyecto
Este proyecto demuestra capacidad técnica sólida en desarrollo frontend moderno, habilidades de trabajo en equipo efectivo y comprensión profunda de los requisitos específicos del dominio (café Santander). La FASE I establece una base excelente para iteraciones futuras y representa un cumplimiento sobresaliente de los objetivos académicos planteados.

📞 Soporte Técnico
Si encuentras problemas durante la instalación:

Revisa la consola del navegador (F12) para errores

Verifica que todas las dependencias estén instaladas

Asegúrate de usar Node.js 18+

Ejecuta npm run type-check para verificar TypeScript

¿Problemas persistentes?

Crea un issue en el repositorio

Verifica la documentación de React y Vite

Consulta las guías de instalación oficiales


<p align="center"> <em>¡Listo para comenzar! Ejecuta `npm run dev` y disfruta de Café Santander 🚀</em> </p><p align="center"> <em>Desarrollado con ❤️ por el Grupo 2 - Diseño de Aplicaciones Web - Universidad Industrial de Santander</em> </p>

<p align="center"> <em>¡Listo para comenzar! Ejecuta `npm run dev` y disfruta de Café Santander 🚀</em> </p><p align="center"> <em>Desarrollado con ❤️ por el Grupo 2 - Diseño de Aplicaciones Web - Universidad Industrial de Santander</em> </p>
