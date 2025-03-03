# Documentación del Proyecto Web (Generada con IA)

## 1. Contenido de las Páginas HTML

### **1.1 index.html** (Inicio)

Esta página sirve como la principal del sitio y contiene:

- Un **navbar** con enlaces a las diferentes secciones.
- Un **carrusel de imágenes** con Bootstrap.
- Una **sección de introducción** que describe los servicios IT con IA.
- Un **artículo destacado** sobre transformación digital.
- Una **barra lateral** con noticias relevantes.
- Secciones con **listas** de beneficios y pasos para comenzar.
- Un **footer** con enlaces legales.

### **1.2 sobre-nosotros.html** (Sobre Nosotros)

Contiene información sobre el equipo y la experiencia:

- Un **banner con carrusel**.
- Secciones sobre **qué hacemos, experiencia, habilidades y objetivos**.
- Uso de listas para habilidades técnicas y blandas.
- **Estilos personalizados** aplicados a cada sección.

### **1.3 servicios.html** (Servicios)

Describe los servicios IT ofrecidos:

- Un **banner con carrusel**.
- Una **introducción** general.
- Sección con **tres servicios principales** en una disposición de tarjetas.
- Una sección de **razones para elegir la empresa**.
- **Estructura con Grid y Flexbox**.

### **1.4 contacto.html** (Contacto)

Página para que los usuarios envíen consultas:

- Un **formulario** con campos para nombre, correo y mensaje.
- Validaciones en los campos.
- Un **botón de envío estilizado**.
- Uso de Flexbox para alineación.

### **1.5 blog.html** (Blog)

Lista de artículos sobre tecnología e IA:

- **Tres publicaciones recientes** en tarjetas.
- Cada tarjeta contiene un **título, descripción y botón de "Leer más"**.
- Uso exclusivo de **Bootstrap** para maquetación.

---

## 2. Aspectos Técnicos

- **Maquetación:** Se usa **Flexbox y Grid** en todas las páginas, excepto en `blog.html`, que utiliza exclusivamente Bootstrap.
- **Componentes de Bootstrap:**
  - Navbar
  - Carrusel (excepto `blog.html` donde también se usa para maquetación general)
- **Modo nocturno:** Implementado con CSS `:has()` y controlado con un checkbox.

---

## 3. Documentación de SASS

### **3.1 Estructura de Archivos**

Los estilos se organizan en `scss/` con subcarpetas:

- `general/` (estructura principal y componentes)
- `utilidades/` (variables, mixins y modo nocturno)

#### **Estructura de Carpetas**

```
/project-root
│── css/ (Archivos compilados de SASS)
│── img/ (Imágenes del sitio)
│── scss/
│   ├── general/
│   │   ├── contenido.scss
│   │   ├── footer.scss
│   │   ├── formularios.scss
│   │   ├── header.scss
│   │   ├── layout.scss
│   │   ├── mq.scss
│   │   ├── reset.scss
│   │   ├── textos.scss
│   ├── utilidades/
│   │   ├── mixins.scss
│   │   ├── modo-nocturno.scss
│   │   ├── modo-nocturno-toggle.scss
│   │   ├── variables.scss
│── html/
│   ├── index.html
│   ├── blog.html
│   ├── contacto.html
│   ├── servicios.html
│   ├── sobre-nosotros.html
│── favicon.ico
│── styles.css
│── README.md
```

### **3.2 Contenido Principal de los Archivos**

#### **variables.scss**

Define colores, breakpoints, bordes, sombras y tipografía.

#### **mixins.scss**

Incluye mixins para:

- **Box-shadow**
- **Breakpoints**
- **Flexbox**

#### **modo-nocturno.scss**

Define los estilos para el modo oscuro.

#### **reset.scss**

Reinicia los estilos base del navegador.

#### **layout.scss**

Define la estructura general con `display: flex` y `grid`.

#### **header.scss**

Estiliza el `navbar` con Bootstrap.

#### **footer.scss**

Define el pie de página con estilos de flexbox.

#### **contenido.scss**

Contiene los estilos de las secciones principales y la barra lateral.

#### **formulario.scss**

Define estilos específicos para formularios y botones de envío.

#### **mq.scss**

Define media queries para dispositivos.

#### **textos.scss**

Define estilos tipográficos.
