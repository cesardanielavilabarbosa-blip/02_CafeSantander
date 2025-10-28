# ☕ Café Santander — FASE I

![React](https://img.shields.io/badge/React-19.0+-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5.5+-3178C6)
![Vite](https://img.shields.io/badge/Vite-5.4+-646CFF)
![Node.js](https://img.shields.io/badge/Node.js-20.0+-brightgreen)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3+-purple)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## **Proyecto: Café Santander — FASE I**

Este repositorio contiene la aplicación web desarrollada en React + TypeScript con Vite para la entrega de la FASE‑I del proyecto.

### **Portada**

**Nombre del aplicativo:** Café Santander  
**02_CafeSantander — FASE I**  
**Aplicación web: Café Santander**

Esta es la entrega de la FASE‑I del proyecto de grupo (Grupo 2). El repositorio contiene la aplicación front‑end desarrollada en React + TypeScript con Vite, la documentación de uso y las instrucciones para empaquetado y entrega.

---

## **Tabla de contenidos**

- [Resumen ejecutivo](#resumen-ejecutivo)
- [Integrantes y roles](#integrantes-y-roles)
- [Objetivos específicos — Lo que hicimos](#objetivos-específicos---lo-que-hicimos)
- [Características principales / Funcionalidades](#características-principales--funcionalidades)
- [Tecnologías utilizadas](#tecnologías-utilizadas)
- [Requisitos previos](#requisitos-previos)
- [Instalación y ejecución local (PowerShell) — paso a paso](#instalación-y-ejecución-local-powershell--paso-a-paso)
- [Estructura del proyecto (árbol) y descripción de carpetas](#estructura-del-proyecto-árbol-y-descripción-de-carpetas)
- [Mecanismo de login y rutas privadas](#mecanismo-de-login-y-rutas-privadas)
- [Formularios y componentes interactivos](#formularios-y-componentes-interactivos)
- [Rueda catadora digital (protótipo)](#rueda-catadora-digital-protótipo)
- [Principios de diseño aplicados (ANEXO 1)](#principios-de-diseño-aplicados-anexo-1)
- [Logros y alcance del proyecto](#logros-y-alcance-del-proyecto)
- [Capturas y demostración](#capturas-y-demostración)
- [Instrucciones para empaquetar y entregar (xx_App.zip)](#instrucciones-para-empaquetar-y-entregar-xx_appzip)
- [Roadmap y próximas mejoras](#roadmap-y-próximas-mejoras)
- [Contribución](#contribución)
- [Contacto de los integrantes](#contacto-de-los-integrantes)

---

## **Resumen ejecutivo**

`02_CafeSantander` es una aplicación front‑end que presenta la identidad y el catálogo de Café Santander. La FASE‑I entregada incluye una interfaz responsiva, navegación con rutas públicas y privadas, formularios, componentes multimedia y un prototipo interactivo de rueda catadora. El objetivo fue entregar una aplicación clara, documentada y lista para ser revisada por el docente.

## **Integrantes y roles**

- **César Daniel Ávila Barbosa (Líder)** — 25% (coordinación y frontend)
- **Juan David Neira Meza** — 25% (componentes y estilos)
- **Nancy Liliana Sáenz Moreno** — 25% (multimedia y pruebas)
- **Carlos David Pimienta Rivera** — 25% (routing y hooks)

## **Objetivos específicos — Lo que hicimos**

1. **Análisis de contexto:** Estudiamos el comercio electrónico del café y documentamos oportunidades para posicionar un producto con identidad local, guiando la selección de contenidos del sitio.
2. **Diseño de flujo de usuario:** Prototipamos un flujo de exploración y compra accesible con catálogo, vista de producto y carrito simulado en frontend.
3. **Interfaz responsiva:** Construimos una interfaz intuitiva adaptable a escritorio, tablet y móvil usando CSS Grid/Flexbox y media queries.
4. **Sistema de autenticación:** Implementamos autenticación simulada mediante modal de Bootstrap (credenciales: Usuario `Admin`, Contraseña `1234`) con protección de rutas privadas.
5. **Rueda catadora digital:** Desarrollamos un prototipo interactivo para ayudar al usuario a seleccionar café según preferencias sensoriales.
6. **Contenido auténtico:** Integramos elementos de la tradición cafetera de Santander como valor diferenciador.
7. **Accesibilidad y usabilidad:** Aplicamos principios de accesibilidad (alt en imágenes, etiquetas en formularios) y protección de rutas.

## **Características principales / Funcionalidades**

- **Diseño responsivo** adaptado a móvil, tablet y desktop
- **Portada** con logo y barra de navegación fija
- **Menú con dropdowns** y navegación intuitiva
- **Rutas públicas y privadas** protegidas con `AuthContext`
- **Modal de login** con Bootstrap y credenciales de prueba
- **Carrito simulado** y vista de productos con tarjetas (`ProductCard`)
- **Formularios** con `react-bootstrap/Form` y validación básica
- **Componentes interactivos:** modales, collapse, popovers, dropdowns, carrusel y acordeón
- **Multimedia:** imágenes, audio y video en carpeta `public/`
- **Footer** con información del equipo y enlaces sociales

## **Tecnologías utilizadas**

- **React (v19)** - Biblioteca principal de interfaz de usuario
- **TypeScript** - Superset tipado de JavaScript
- **Vite** - Herramienta de construcción y desarrollo
- **React Router (v7)** - Manejo de rutas y navegación
- **Bootstrap 5 + React-Bootstrap** - Framework de estilos y componentes
- **ESLint / TypeScript** - Herramientas de calidad de código
- **Node.js / npm** - Entorno de ejecución y gestor de paquetes

**NOTA:** Se eligió TypeScript por ser el estándar actual en desarrollo web con React, ofreciendo tipado estático, detección temprana de errores y mayor escalabilidad, lo que mejora la estabilidad y mantenibilidad de la aplicación frente a JavaScript.

## **Requisitos previos**

- Node.js v18+ (recomendado)
- npm v9+ (recomendado)
- Git
- Navegador moderno (Chrome, Firefox, Safari, Edge)

## **Instalación y ejecución local (PowerShell) — paso a paso**

Ejecuta los siguientes comandos en PowerShell desde tu máquina:

```powershell
# 1. Clonar el repositorio y entrar a la carpeta del proyecto
git clone https://github.com/<usuario>/<repositorio>.git
cd 02_CafeSantander\cafe-react

# 2. Instalar dependencias
npm install

# 3. Ejecutar modo desarrollo (Vite)
npm run dev

# 4. Para producción: construir y previsualizar
npm run build
npm run preview
Después de npm run dev abre la URL que Vite indique (generalmente http://localhost:5173).

Estructura del proyecto (árbol) y descripción de carpetas
text
02_CafeSantander/
└─ cafe-react/
   ├─ .gitignore
   ├─ index.html
   ├─ package.json
   ├─ package-lock.json
   ├─ node_modules/ (no commiteada normalmente)
   ├─ public/
   │  ├─ imagenes/  (logos, fotos)
   │  ├─ audio/
   │  └─ video/
   ├─ src/
   │  ├─ assets/    (imágenes y recursos importados)
   │  ├─ components/ (Header, Footer, Modales, ProductCard, PrivateRoute)
   │  ├─ context/    (AuthContext.tsx)
   │  ├─ hooks/      (useCart y hooks personalizados)
   │  ├─ pages/      (Inicio, Productos, Carrito, Contacto, Acerca, Servicios)
   │  ├─ styles/     (css por página y global)
   │  ├─ App.css
   │  ├─ App.tsx
   │  ├─ index.css
   │  ├─ main.tsx
   │  └─ (otros archivos TypeScript/JS según componentes)
   ├─ tsconfig.json
   ├─ tsconfig.app.json
   ├─ tsconfig.node.json
   └─ vite.config.ts
Descripción de carpetas clave
public/: recursos estáticos que se sirven directamente (imágenes, audio, video)

src/: código fuente principal de la aplicación

components/: componentes React reutilizables (Header, Footer, modales, tarjetas)

pages/: vistas que representan cada página del sitio

context/: contextos React (AuthContext para autenticación)

hooks/: hooks personalizados (ej. useCart)

styles/: archivos CSS organizados por página o globales

assets/: imágenes y recursos importados desde TypeScript/JS

Mecanismo de login y rutas privadas
Modal de login: src/components/BootstrapLoginModal.tsx

Contexto de autenticación: src/context/AuthContext.tsx

Protección de rutas: src/components/PrivateRoute.tsx

Credenciales de evaluación (simulación):

Usuario: Admin

Contraseña: 1234

Flujo de autenticación: Al iniciar sesión con las credenciales, AuthContext actualiza el estado a autenticado y las rutas privadas se vuelven accesibles. PrivateRoute impide el acceso directo por URL cuando el usuario no está autenticado.

Formularios y componentes interactivos
Formularios: src/pages/Contacto.tsx usa react-bootstrap/Form con validación básica

Componentes interactivos: Carrusel, Acordeón, Collapse, Popover y Dropdown mediante react-bootstrap

Multimedia: Archivos en public/video/ y public/audio/ con controles de reproducción

Rueda catadora digital (protótipo)
Se incluyó un prototipo de rueda catadora en la sección de Productos/Servicios para orientar la selección del café con base en preferencias sensoriales (sabor, aroma, intensidad). El componente es interactivo y sirve como base para futuras mejoras.

Principios de diseño aplicados (ANEXO 1)
Contraste de color para legibilidad óptima

Jerarquía visual mediante tipografías y espaciado consistente

Consistencia visual con componentes reutilizables

Accesibilidad básica: alt en imágenes, labels en formularios y foco visible

Usabilidad: barra de navegación fija y estructura clara de contenidos

Logros y alcance del proyecto
✅ Interfaz responsiva y navegable en distintos dispositivos

✅ Rutas públicas y privadas con autenticación simulada funcional

✅ Formularios y validaciones básicas implementadas

✅ Componentes interactivos y multimedia integrados

✅ Prototipo de rueda catadora digital operativo

✅ Documentación completa para instalación y ejecución

Capturas y demostración
Las siguientes capturas corresponden a pantallas principales de la aplicación:

https:///imagenes/cafe/portada-1.png
Portada y header con menú de navegación

https:///imagenes/cafe/login-modal.png
Modal de inicio de sesión con credenciales de prueba

https:///imagenes/cafe/ruleta-catadora.png
Rueda catadora interactiva en página de Servicios

https:///imagenes/cafe/historia.png
Sección "Nuestra Historia" con banner principal

https:///imagenes/cafe/productos.png
Catálogo de productos con tarjetas interactivas

Para ver las capturas localmente: Coloca las imágenes en public/imagenes/cafe/ y accede mediante http://localhost:5173/imagenes/cafe/ cuando el servidor de desarrollo esté activo.

Instrucciones para empaquetar y entregar (xx_App.zip)
Construir la aplicación:

powershell
npm run build
Preparar carpeta de entrega:

Crear carpeta 02_App

Copiar carpeta cafe-react completa sin node_modules

Incluir archivo 02_aplicativo.pdf con portada, capturas y anexos

Agregar Readme.txt con versión resumida de este README

Empaquetar y entregar:

Comprimir la carpeta 02_App en 02_App.zip

Subir a la plataforma académica o proporcionar enlace al docente

Recomendación: Incluir la carpeta dist/ en el zip para que el docente pueda ver la versión construida sin ejecutar npm install.

Roadmap y próximas mejoras
todoooooooooooooooooooo
☕ Café Santander — FASE I
https://img.shields.io/badge/React-19.0+-blue
https://img.shields.io/badge/TypeScript-5.5+-3178C6
https://img.shields.io/badge/Vite-5.4+-646CFF
https://img.shields.io/badge/Node.js-20.0+-brightgreen
https://img.shields.io/badge/Bootstrap-5.3+-purple
https://img.shields.io/badge/License-MIT-yellow

Proyecto: Café Santander — FASE I
Este repositorio contiene la aplicación web desarrollada en React + TypeScript con Vite para la entrega de la FASE‑I del proyecto.

Portada
Nombre del aplicativo: Café Santander
02_CafeSantander — FASE I
Aplicación web: Café Santander

Esta es la entrega de la FASE‑I del proyecto de grupo (Grupo 2). El repositorio contiene la aplicación front‑end desarrollada en React + TypeScript con Vite, la documentación de uso y las instrucciones para empaquetado y entrega.

Tabla de contenidos
Resumen ejecutivo

Integrantes y roles

Objetivos específicos — Lo que hicimos

Características principales / Funcionalidades

Tecnologías utilizadas

Requisitos previos

Instalación y ejecución local (PowerShell) — paso a paso

Estructura del proyecto (árbol) y descripción de carpetas

Mecanismo de login y rutas privadas

Formularios y componentes interactivos

Rueda catadora digital (protótipo)

Principios de diseño aplicados (ANEXO 1)

Logros y alcance del proyecto

Capturas y demostración

Instrucciones para empaquetar y entregar (xx_App.zip)

Roadmap y próximas mejoras

Contribución

Contacto de los integrantes

Conclusiones del Proyecto

Resumen ejecutivo
02_CafeSantander es una aplicación front‑end que presenta la identidad y el catálogo de Café Santander. La FASE‑I entregada incluye una interfaz responsiva, navegación con rutas públicas y privadas, formularios, componentes multimedia y un prototipo interactivo de rueda catadora. El objetivo fue entregar una aplicación clara, documentada y lista para ser revisada por el docente.

Integrantes y roles
César Daniel Ávila Barbosa (Líder) — 25% (coordinación y frontend)

Juan David Neira Meza — 25% (componentes y estilos)

Nancy Liliana Sáenz Moreno — 25% (multimedia y pruebas)

Carlos David Pimienta Rivera — 25% (routing y hooks)

Objetivos específicos — Lo que hicimos
Análisis de contexto: Estudiamos el comercio electrónico del café y documentamos oportunidades para posicionar un producto con identidad local, guiando la selección de contenidos del sitio.

Diseño de flujo de usuario: Prototipamos un flujo de exploración y compra accesible con catálogo, vista de producto y carrito simulado en frontend.

Interfaz responsiva: Construimos una interfaz intuitiva adaptable a escritorio, tablet y móvil usando CSS Grid/Flexbox y media queries.

Sistema de autenticación: Implementamos autenticación simulada mediante modal de Bootstrap (credenciales: Usuario Admin, Contraseña 1234) con protección de rutas privadas.

Rueda catadora digital: Desarrollamos un prototipo interactivo para ayudar al usuario a seleccionar café según preferencias sensoriales.

Contenido auténtico: Integramos elementos de la tradición cafetera de Santander como valor diferenciador.

Accesibilidad y usabilidad: Aplicamos principios de accesibilidad (alt en imágenes, etiquetas en formularios) y protección de rutas.

Características principales / Funcionalidades
Diseño responsivo adaptado a móvil, tablet y desktop

Portada con logo y barra de navegación fija

Menú con dropdowns y navegación intuitiva

Rutas públicas y privadas protegidas con AuthContext

Modal de login con Bootstrap y credenciales de prueba

Carrito simulado y vista de productos con tarjetas (ProductCard)

Formularios con react-bootstrap/Form y validación básica

Componentes interactivos: modales, collapse, popovers, dropdowns, carrusel y acordeón

Multimedia: imágenes, audio y video en carpeta public/

Footer con información del equipo y enlaces sociales

Tecnologías utilizadas
React (v19) - Biblioteca principal de interfaz de usuario

TypeScript - Superset tipado de JavaScript

Vite - Herramienta de construcción y desarrollo

React Router (v7) - Manejo de rutas y navegación

Bootstrap 5 + React-Bootstrap - Framework de estilos y componentes

ESLint / TypeScript - Herramientas de calidad de código

Node.js / npm - Entorno de ejecución y gestor de paquetes

NOTA: Se eligió TypeScript por ser el estándar actual en desarrollo web con React, ofreciendo tipado estático, detección temprana de errores y mayor escalabilidad, lo que mejora la estabilidad y mantenibilidad de la aplicación frente a JavaScript.

Requisitos previos
Node.js v18+ (recomendado)

npm v9+ (recomendado)

Git

Navegador moderno (Chrome, Firefox, Safari, Edge)

Instalación y ejecución local (PowerShell) — paso a paso
Ejecuta los siguientes comandos en PowerShell desde tu máquina:

powershell
# 1. Clonar el repositorio y entrar a la carpeta del proyecto
git clone https://github.com/<usuario>/<repositorio>.git
cd 02_CafeSantander\cafe-react

# 2. Instalar dependencias
npm install

# 3. Ejecutar modo desarrollo (Vite)
npm run dev

# 4. Para producción: construir y previsualizar
npm run build
npm run preview
Después de npm run dev abre la URL que Vite indique (generalmente http://localhost:5173).

Estructura del proyecto (árbol) y descripción de carpetas
text
02_CafeSantander/
└─ cafe-react/
   ├─ .gitignore
   ├─ index.html
   ├─ package.json
   ├─ package-lock.json
   ├─ node_modules/ (no commiteada normalmente)
   ├─ public/
   │  ├─ imagenes/  (logos, fotos)
   │  ├─ audio/
   │  └─ video/
   ├─ src/
   │  ├─ assets/    (imágenes y recursos importados)
   │  ├─ components/ (Header, Footer, Modales, ProductCard, PrivateRoute)
   │  ├─ context/    (AuthContext.tsx)
   │  ├─ hooks/      (useCart y hooks personalizados)
   │  ├─ pages/      (Inicio, Productos, Carrito, Contacto, Acerca, Servicios)
   │  ├─ styles/     (css por página y global)
   │  ├─ App.css
   │  ├─ App.tsx
   │  ├─ index.css
   │  ├─ main.tsx
   │  └─ (otros archivos TypeScript/JS según componentes)
   ├─ tsconfig.json
   ├─ tsconfig.app.json
   ├─ tsconfig.node.json
   └─ vite.config.ts
Descripción de carpetas clave
public/: recursos estáticos que se sirven directamente (imágenes, audio, video)

src/: código fuente principal de la aplicación

components/: componentes React reutilizables (Header, Footer, modales, tarjetas)

pages/: vistas que representan cada página del sitio

context/: contextos React (AuthContext para autenticación)

hooks/: hooks personalizados (ej. useCart)

styles/: archivos CSS organizados por página o globales

assets/: imágenes y recursos importados desde TypeScript/JS

Mecanismo de login y rutas privadas
Modal de login: src/components/BootstrapLoginModal.tsx

Contexto de autenticación: src/context/AuthContext.tsx

Protección de rutas: src/components/PrivateRoute.tsx

Credenciales de evaluación (simulación):

Usuario: Admin

Contraseña: 1234

Flujo de autenticación: Al iniciar sesión con las credenciales, AuthContext actualiza el estado a autenticado y las rutas privadas se vuelven accesibles. PrivateRoute impide el acceso directo por URL cuando el usuario no está autenticado.

Formularios y componentes interactivos
Formularios: src/pages/Contacto.tsx usa react-bootstrap/Form con validación básica

Componentes interactivos: Carrusel, Acordeón, Collapse, Popover y Dropdown mediante react-bootstrap

Multimedia: Archivos en public/video/ y public/audio/ con controles de reproducción

Rueda catadora digital (protótipo)
Se incluyó un prototipo de rueda catadora en la sección de Productos/Servicios para orientar la selección del café con base en preferencias sensoriales (sabor, aroma, intensidad). El componente es interactivo y sirve como base para futuras mejoras.

Principios de diseño aplicados (ANEXO 1)
Contraste de color para legibilidad óptima

Jerarquía visual mediante tipografías y espaciado consistente

Consistencia visual con componentes reutilizables

Accesibilidad básica: alt en imágenes, labels en formularios y foco visible

Usabilidad: barra de navegación fija y estructura clara de contenidos

Logros y alcance del proyecto
✅ Interfaz responsiva y navegable en distintos dispositivos

✅ Rutas públicas y privadas con autenticación simulada funcional

✅ Formularios y validaciones básicas implementadas

✅ Componentes interactivos y multimedia integrados

✅ Prototipo de rueda catadora digital operativo

✅ Documentación completa para instalación y ejecución

Capturas y demostración
Las siguientes capturas corresponden a pantallas principales de la aplicación:

https:///imagenes/cafe/portada-1.png
Portada y header con menú de navegación

https:///imagenes/cafe/login-modal.png
Modal de inicio de sesión con credenciales de prueba

https:///imagenes/cafe/ruleta-catadora.png
Rueda catadora interactiva en página de Servicios

https:///imagenes/cafe/historia.png
Sección "Nuestra Historia" con banner principal

https:///imagenes/cafe/productos.png
Catálogo de productos con tarjetas interactivas

Para ver las capturas localmente: Coloca las imágenes en public/imagenes/cafe/ y accede mediante http://localhost:5173/imagenes/cafe/ cuando el servidor de desarrollo esté activo.

Instrucciones para empaquetar y entregar (xx_App.zip)
Construir la aplicación:

powershell
npm run build
Preparar carpeta de entrega:

Crear carpeta 02_App

Copiar carpeta cafe-react completa sin node_modules

Incluir archivo 02_aplicativo.pdf con portada, capturas y anexos

Agregar Readme.txt con versión resumida de este README

Empaquetar y entregar:

Comprimir la carpeta 02_App en 02_App.zip

Subir a la plataforma académica o proporcionar enlace al docente

Recomendación: Incluir la carpeta dist/ en el zip para que el docente pueda ver la versión construida sin ejecutar npm install.

Roadmap y próximas mejoras
Integración backend: Autenticación real y persistencia en base de datos

Sistema de encuestas: Módulo de encuestas con estadísticas integradas

Mejora de rueda catadora: Datos sensoriales guardados por usuario

Validaciones robustas: Implementación de captcha y validaciones avanzadas en formularios

Panel de administración: Gestión de productos y usuarios

Pasarela de pagos: Integración con sistemas de pago en línea

Contribución
Si deseas colaborar:

Fork del proyecto

Clonar tu fork y crear una rama feature

Realizar cambios y pruebas

Enviar Pull Request con descripción clara

Convenciones de commits: feat:, fix:, docs:, style:, refactor:, test:

Contacto de los integrantes
César Daniel Ávila Barbosa — cesar2224642@correo.uis.edu.co— 25%

Juan David Neira Meza — juan2235605@correo.uis.edu.co — 25%

Nancy Liliana Sáenz Moreno — nancy2224510@correo.uis.edu.co — 25%

Carlos David Pimienta Rivera — carlos2221873@correo.uis.edu.co — 25%

Conclusiones del Proyecto
✅ Logros Destacados
Arquitectura Técnica Sólida:

Implementación exitosa de React + TypeScript + Vite como stack tecnológico moderno

Uso de TypeScript que garantiza mayor robustez y mantenibilidad del código

Configuración eficiente del entorno de desarrollo con Vite para mejor performance

Distribución Equitativa de Responsabilidades:

División clara y balanceada del trabajo (25% por integrante)

Roles especializados definidos: coordinación, frontend, componentes, estilos, multimedia, routing

Enfoque colaborativo que permite aprovechar las fortalezas individuales

Estructura de Proyecto Bien Organizada:

Documentación completa con tabla de contenidos detallada

Instrucciones claras de instalación y ejecución

Enfoque en buenas prácticas de desarrollo y mantenibilidad

🔧 Aspectos Técnicos Relevantes
Características Implementadas:

Sistema de autenticación funcional con mecanismo de login

Implementación completa de rutas privadas protegidas

Formularios y componentes interactivos responsivos

Prototipo de rueda catadora digital (valor agregado específico del dominio cafetero)

Enfoque en UX/UI:

Aplicación consistente de principios de diseño (ANEXO 1)

Desarrollo de componentes reutilizables y modulares

Atención meticulosa a estilos y experiencia de usuario

👥 Fortalezas del Equipo
Colaboración Efectiva:

Coordinación clara bajo el liderazgo definido

Especialización en áreas complementarias del desarrollo

Distribución equilibrada de carga de trabajo

Alineación con Objetivos Académicos:

Cumplimiento integral de requisitos del curso "Diseño de Aplicaciones Web"

Aplicación práctica de conceptos teóricos en proyecto real

Entrega completa dentro del plazo establecido

🚀 Potencial de Evolución
Base Sólida para Fases Futuras:

Arquitectura escalable preparada para nuevas funcionalidades

Documentación que facilita la continuidad del proyecto

Prototipo funcional que valida el concepto central del negocio

Oportunidades de Mejora Identificadas:

La rueda catadora digital como prototipo sugiere espacio para desarrollo adicional

Posible expansión de funcionalidades interactivas y multimedia

Optimización de componentes existentes para mejor performance

💡 Valor del Proyecto
Este proyecto demuestra capacidad técnica sólida en desarrollo frontend moderno, habilidades de trabajo en equipo efectivo y comprensión profunda de los requisitos específicos del dominio (café Santander). La FASE I establece una base excelente para iteraciones futuras y representa un cumplimiento sobresaliente de los objetivos académicos planteados.

<p align="center"> <em>Desarrollado con ❤️ por el Grupo 2 - Diseño de Aplicaciones Web - Universidad Industrial de Santander</em> </p>
