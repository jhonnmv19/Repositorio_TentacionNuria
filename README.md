# 📘 Repositorio Tentación de Nuria - Versión HTML/CSS

Este proyecto es el **Repositorio Tentación de Nuria**, un sistema digital creado para organizar, almacenar y visualizar todas las recetas desarrolladas a lo largo de los módulos de formación culinaria.

Está hecho con **HTML, CSS y JavaScript puro**, pensado para ser sencillo, bonito y totalmente responsive, ideal para uso familiar y práctico.

---

## 📂 Estructura del Proyecto

```
Repositorio-Tentacion-de-Nuria/
│
├── index.html                    # Página principal
│
├── paginas/
│   ├── menu.html                 # Vista de todos los módulos
│   ├── contacto.html             # Página de contacto
│   └── sobre-nosotros.html       # Información del proyecto
│
├── modulos/
│   ├── modulo1.html              # Listado de recetas del módulo 1
│   ├── modulo2.html              # Listado de recetas del módulo 2
│   ├── modulo3.html              # Listado de recetas del módulo 3
│   ├── modulo4.html              # Listado de recetas del módulo 4
│   ├── modulo5.html              # Listado de recetas del módulo 5
│   └── modulo6.html              # Listado de recetas del módulo 6
│
├── detallesM1/
│   ├── receta1.html              # Detalle de receta 1 del módulo 1
│   ├── receta2.html              # Detalle de receta 2 del módulo 1
│   └── ...                       # (hasta 35 recetas)
│
├── detallesM2/
│   └── ...                       # Recetas del módulo 2
│
├── detallesM3/
│   └── ...                       # Recetas del módulo 3
│
├── detallesM4/
│   └── ...                       # Recetas del módulo 4
│
├── detallesM5/
│   └── ...                       # Recetas del módulo 5
│
├── detallesM6/
│   └── ...                       # Recetas del módulo 6
│
├── estilos/
│   └── estilo.css                # Archivo CSS principal
│
├── js/
│   └── script.js                 # JavaScript para interactividad
│
└── imagenes/
    └── (tus imágenes personales)  # Carpeta para imágenes propias
```

---

## 🎨 Diseño y Paleta de Colores

El estilo visual utiliza los siguientes colores:

- **Header**: `#bc6071`
- **Botones**: `#e49dab`
- **Secciones destacadas**: `#cca0a8`
- **Hover**: `#a4202e`
- **Fondo general**: `#fefae2`

Diseño moderno, limpio y agradable para la vista.

---

## 📑 Descripción de las Páginas

### 🏠 index.html
- Página principal con bienvenida
- Logo de Tentación de Nuria
- Navegación principal
- Llamada a la acción para explorar módulos

### 📜 paginas/menu.html
- Vista de todos los 6 módulos disponibles
- Cada módulo indica cuántas recetas contiene

### 📁 modulos/moduloX.html
- Listados de recetas del módulo X
- Cada receta incluye:
  - Imagen
  - Nombre
  - Descripción breve
  - Botón "Ver más"

### 🍰 detallesM1/recetaX.html
- Página detallada de cada receta:
  - Nombre de la receta
  - Imagen principal
  - Ingredientes con checkmarks
  - Preparación paso a paso numerada
  - Decoración, relleno o notas (si la receta lo requiere)
  - Botón "Volver al módulo"

### 📞 paginas/contacto.html
- Incluye botones para:
  - WhatsApp (con enlace directo)
  - Email
  - Teléfono
- **Nota**: Debes reemplazar `34XXXXXXXXX` con tu número real

### 👥 paginas/sobre-nosotros.html
- Presenta:
  - Historia
  - Visión
  - Valores
  - Nuestro equipo
  - Estadísticas

---

## 📱 Responsividad

El sitio está optimizado para:
- ✅ Celulares
- ✅ Tablets
- ✅ Computadoras

Con diseño flexible y adaptable mediante **CSS Grid** y **Flexbox**.

---

## 🖼 Imágenes

### Imágenes Actuales
- Las imágenes actualmente usan **Unsplash** (servicio gratuito de imágenes)
- URLs tipo: `https://source.unsplash.com/400x300/?chocolate,cake`

### Usar Imágenes Propias
Para usar tus propias imágenes:

1. Guarda tus imágenes en la carpeta `imagenes/`
2. Usa nombres descriptivos: `tarta-chocolate.jpg`, `galletas-mantequilla.jpg`
3. Reemplaza las URLs en los archivos HTML:

```html
<!-- Antes (Unsplash) -->
<img src="https://source.unsplash.com/400x300/?chocolate,cake" alt="...">

<!-- Después (imagen propia) -->
<img src="../imagenes/tarta-chocolate.jpg" alt="...">
```

---

## 🔧 Cómo Agregar Nuevas Recetas

### Paso 1: Crear archivo de detalle
1. Ve a la carpeta correspondiente (ej: `detallesM1/`)
2. Crea nuevo archivo: `receta3.html`, `receta4.html`, etc.
3. Copia el contenido de `receta1.html` o `receta2.html`
4. Modifica:
   - Título de la página (`<title>`)
   - Nombre de la receta
   - Imagen
   - Ingredientes
   - Preparación
   - Decoración (si aplica)
   - Notas (si aplica)

### Paso 2: Agregar al módulo
1. Abre el archivo del módulo (ej: `modulos/modulo1.html`)
2. Agrega una nueva tarjeta de receta:

```html
<a href="../detallesM1/receta3.html" class="receta-card">
    <div class="card">
        <img src="../imagenes/tu-imagen.jpg" alt="Nombre de Receta" class="receta-imagen">
        <div class="receta-contenido">
            <h3 class="receta-nombre">Nombre de la Receta</h3>
            <p class="receta-descripcion">Descripción breve</p>
            <span class="btn btn-secondary">Ver más</span>
        </div>
    </div>
</a>
```

---

## 🌐 Cómo Ver el Sitio

### En tu computadora (local):
1. Abre el archivo `index.html` con tu navegador
2. Navega por todas las páginas

### Publicar en Internet:
Puedes subir todos los archivos a servicios gratuitos como:
- **GitHub Pages** (gratis, recomendado)
- **Netlify** (gratis)
- **Vercel** (gratis)
- Cualquier hosting web

---

## ⚙️ Personalización

### Cambiar Colores
Edita el archivo `estilos/estilo.css` en las variables CSS:

```css
:root {
  --color-header: #bc6071;      /* Color del header */
  --color-button: #e49dab;      /* Color de botones */
  --color-section: #cca0a8;     /* Secciones destacadas */
  --color-hover: #a4202e;       /* Efecto hover */
  --color-bg: #fefae2;          /* Fondo general */
}
```

### Cambiar Logo
Reemplaza la URL del logo en todos los archivos HTML:

```html
<img src="TU_IMAGEN_LOGO" alt="Tentación de Nuria Logo" class="logo-img">
```

### Actualizar Número de WhatsApp
En `paginas/contacto.html`, busca y reemplaza:

```html
<!-- Busca -->
https://wa.me/34XXXXXXXXX

<!-- Reemplaza con tu número (con código país, sin espacios) -->
https://wa.me/34612345678
```

---

## 📌 Footer

Todas las páginas tienen el footer:
```
Repositorio Tentación de Nuria — 2025
```

Para cambiar el año, edita el texto en cada archivo HTML o usa JavaScript para auto-actualizar.

---

## 🎯 Objetivo del Repositorio

El Repositorio Tentación de Nuria fue creado para:
- ✅ Tener un archivo digital organizado
- ✅ Consultar recetas de forma rápida
- ✅ Facilitar el trabajo familiar
- ✅ Servir como catálogo de recetas preparadas
- ✅ Mantener ordenadas las recetas por módulos

---

## 📊 Contenido Completo

- **6 Módulos** de formación culinaria
- **~35 recetas por módulo** (210 recetas en total)
- Cada receta con:
  - Ingredientes detallados
  - Pasos de preparación
  - Decoración (cuando aplica)
  - Notas especiales (cuando aplica)

---

## 💡 Consejos Técnicos

1. **Mantén la estructura de carpetas**: Es importante para que los enlaces funcionen
2. **Usa rutas relativas**: Los `../` son necesarios para navegar entre carpetas
3. **Optimiza imágenes**: Usa imágenes de máximo 800KB para carga rápida
4. **Prueba en móvil**: Abre el sitio en tu teléfono para verificar responsividad
5. **Haz backup**: Guarda copias de tus archivos regularmente

---

## 🚀 Próximos Pasos Sugeridos

1. ✅ Completa las 35 recetas de cada módulo
2. ✅ Reemplaza imágenes de Unsplash con fotos propias
3. ✅ Actualiza el número de WhatsApp en contacto
4. ✅ Personaliza textos en "Sobre Nosotros"
5. ✅ Considera agregar un buscador de recetas (JavaScript)
6. ✅ Agrega botones de imprimir receta
7. ✅ Añade una sección de recetas favoritas

---

## 📝 Plantilla de Receta Rápida

Para copiar y pegar al crear nuevas recetas:

```html
<li><span class="check-icon">✓</span><span>Ingrediente aquí</span></li>
```

```html
<li><span class="step-number"></span><p>Paso de preparación aquí</p></li>
```

```html
<li><span class="star-icon">★</span><span>Decoración aquí</span></li>
```

---

## ❤️ Hecho con Amor

Este proyecto está diseñado para ser simple, elegante y funcional.
Cada página ha sido creada pensando en la mejor experiencia de usuario.

**Repositorio Tentación de Nuria — 2025**

---

## 📧 Soporte

Si tienes dudas sobre cómo usar o modificar el proyecto, revisa este README o los archivos HTML como ejemplos.

¡Disfruta organizando tus recetas! 👨‍🍳❤️
