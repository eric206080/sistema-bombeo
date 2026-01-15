# 🚀 INGDELCA - Landing Page
## Soluciones de Bombeo Industrial en Perú

![INGDELCA Logo](images/logo.png)

Landing page profesional para INGDELCA, empresa especializada en aplicaciones de bombeo industrial, agroindustrial, PTAR y proyectos especiales en Perú.

---

## 📋 Descripción

Landing page moderna y responsive diseñada para generar leads B2B a través de WhatsApp. Enfocada en conversión con múltiples CTAs estratégicos y contenido técnico optimizado para SEO.

### ✨ Características Principales

- 🎯 **Enfoque en conversión**: 8+ botones de WhatsApp con mensajes prellenados
- 📱 **100% Responsive**: Optimizado para móvil, tablet y desktop
- ⚡ **Carga rápida**: HTML/CSS puro, sin dependencias pesadas
- 🔍 **SEO Optimizado**: Meta tags, estructura semántica, keywords
- 🎨 **Diseño profesional**: Colores corporativos, tipografía moderna
- 📊 **Formulario de contacto**: Integración con FormSpree
- ❓ **FAQs técnicas**: 8 preguntas frecuentes expandibles
- 🏆 **Credibilidad**: Secciones de confianza y diferenciadores

---

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos con variables CSS
- **Google Fonts**: Tipografía Inter
- **FormSpree**: Gestión de formularios (opcional)

---

## 📁 Estructura del Proyecto

```
ingdelca-project/
│
├── index.html              # Página principal
├── README.md               # Este archivo
├── .gitignore             # Archivos ignorados por Git
│
├── css/
│   └── styles.css         # Estilos principales
│
├── images/
│   ├── logo.png           # Logo INGDELCA
│   ├── hero-pumps.jpg     # Imagen hero (agregar)
│   ├── sector-industria.jpg    # (agregar)
│   ├── sector-agro.jpg         # (agregar)
│   ├── sector-ptar.jpg         # (agregar)
│   └── sector-proyectos.jpg    # (agregar)
│
└── js/
    └── (vacío - para futuras mejoras)
```

---

## 🚀 Instalación y Uso

### **Opción 1: Uso Local**

1. **Clonar el repositorio:**
```bash
git clone https://github.com/TU-USUARIO/ingdelca-landing.git
cd ingdelca-landing
```

2. **Abrir en navegador:**
```bash
# Simplemente abre index.html en tu navegador
# O usa un servidor local:
python -m http.server 8000
# Luego visita: http://localhost:8000
```

### **Opción 2: Subir a Hosting**

1. **Conectar vía FTP** (FileZilla, WinSCP, etc.)
2. **Subir todos los archivos** a la carpeta `/public_html/`
3. **Configurar SSL** en el panel de hosting
4. **¡Listo!** Tu sitio estará en: `https://tudominio.com`

### **Opción 3: GitHub Pages (Gratis)**

1. **Push a GitHub:**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/ingdelca-landing.git
git push -u origin main
```

2. **Habilitar GitHub Pages:**
   - Ve a Settings → Pages
   - Source: Deploy from branch
   - Branch: main / (root)
   - Save

3. **Tu sitio estará en:**
   `https://TU-USUARIO.github.io/ingdelca-landing/`

---

## ⚙️ Configuración

### **1. Actualizar Datos de Contacto**

Busca y reemplaza en `index.html`:

```html
<!-- WhatsApp -->
https://wa.me/51948579939
→ Reemplazar con tu número

<!-- Email -->
comercial@ingdelca.com
→ Reemplazar con tu email
```

### **2. Configurar Formulario**

El formulario usa FormSpree. Para activarlo:

1. Ve a [formspree.io](https://formspree.io)
2. Crea cuenta gratis
3. Crea nuevo formulario
4. Copia el endpoint que te dan
5. En `index.html`, busca:
```html
<form action="https://formspree.io/f/XXXXXXXX" method="POST">
```
6. Reemplaza `XXXXXXXX` con tu código

### **3. Agregar Google Analytics**

Antes de `</head>` en `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### **4. Agregar Imágenes**

Coloca tus imágenes en la carpeta `/images/` con estos nombres:
- `hero-pumps.jpg` (1200x800px)
- `sector-industria.jpg` (800x600px)
- `sector-agro.jpg` (800x600px)
- `sector-ptar.jpg` (800x600px)
- `sector-proyectos.jpg` (800x600px)

---

## 🎨 Personalización

### **Cambiar Colores**

Edita las variables CSS en `css/styles.css`:

```css
:root {
    --primary-color: #0e4c92;      /* Azul principal */
    --primary-dark: #0a3a6f;       /* Azul oscuro */
    --secondary-color: #1a9dd9;    /* Azul claro */
    --accent-color: #FF6B00;       /* Naranja */
}
```

### **Modificar Textos**

Todos los textos están en `index.html`. Busca las secciones:
- Hero
- Sectores
- Servicios
- Proceso
- FAQs
- etc.

---

## 📊 Secciones de la Landing Page

1. **Navbar**: Logo + contacto + CTA
2. **Hero**: Propuesta de valor + beneficios + CTAs
3. **Trust Band**: Credibilidad inicial
4. **Promesa**: Garantía 24-48h
5. **Sectores**: 4 sectores industriales
6. **Servicios**: 3 servicios principales
7. **Proceso**: 4 pasos del trabajo
8. **Diferenciadores**: 6 ventajas competitivas
9. **Formulario**: Captura de leads + WhatsApp
10. **FAQs**: 8 preguntas frecuentes
11. **Trust Final**: 6 elementos de confianza
12. **Footer**: Información completa

---

## 🔧 Mantenimiento

### **Actualizar Contenido**
- Editar `index.html` directamente
- Subir cambios vía FTP o Git

### **Actualizar Estilos**
- Editar `css/styles.css`
- Los cambios se reflejan automáticamente

### **Optimizar Imágenes**
- Usa herramientas como TinyPNG
- Formato recomendado: WebP o JPG optimizado
- Tamaño máximo: 200KB por imagen

---

## 📱 Responsive Breakpoints

- **Desktop**: > 992px
- **Tablet**: 768px - 992px
- **Mobile**: < 768px
- **Small Mobile**: < 480px

---

## 🚨 Solución de Problemas

### **Las imágenes no cargan**
- Verificar rutas en `index.html`
- Asegurar que archivos existen en `/images/`
- Revisar nombres de archivos (case-sensitive)

### **WhatsApp no abre**
- Verificar formato de número: `51948579939`
- Sin espacios, guiones o caracteres especiales
- Incluir código de país: `51`

### **Formulario no envía**
- Configurar FormSpree correctamente
- Verificar endpoint en `<form action="">`
- Revisar spam en email

---

## 📈 SEO

### **Meta Tags Incluidos**
- Title
- Description
- Keywords
- Open Graph
- Favicon

### **Mejoras Sugeridas**
1. Agregar Schema.org markup
2. Sitemap.xml
3. Robots.txt
4. Blog con contenido técnico
5. Backlinks de calidad

---

## 🔐 Seguridad

- ✅ SSL/HTTPS requerido
- ✅ FormSpree protege de spam
- ✅ No hay almacenamiento de datos sensibles
- ✅ Código limpio sin vulnerabilidades

---

## 📝 Licencia

Este proyecto es propiedad de **INGDELCA - Ingeniería & Consultoría**.

Todos los derechos reservados © 2025

---

## 👨‍💻 Desarrollo

**Desarrollado por:** [Tu Nombre/Empresa]  
**Para:** INGDELCA  
**Año:** 2025

---

## 📞 Soporte

¿Preguntas o problemas?

- 📱 WhatsApp: +51 948 579 939
- 📧 Email: comercial@ingdelca.com

---

## 🎯 Próximas Mejoras

- [ ] Blog técnico
- [ ] Calculadora TDH interactiva
- [ ] Galería de proyectos
- [ ] Testimonios en video
- [ ] Chat en vivo
- [ ] Modo oscuro
- [ ] Multiidioma (EN)

---

## ⭐ Si te gusta este proyecto

¡Dale una estrella en GitHub! ⭐

---

**Hecho con ❤️ para INGDELCA**
