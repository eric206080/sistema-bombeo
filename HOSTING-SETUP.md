# 🌐 GUÍA COMPLETA: SUBIR AL HOSTING

## 📋 REQUISITOS
- ✅ Hosting contratado (Hostinger, SiteGround, etc.)
- ✅ Dominio configurado
- ✅ Archivos del proyecto descargados

---

## 📂 PREPARACIÓN DE ARCHIVOS

### **ANTES DE SUBIR:**

1. **Verificar datos de contacto actualizados:**
   - WhatsApp: `+51 948 579 939` ✅
   - Email: `comercial@ingdelca.com` ✅

2. **Agregar tus imágenes:**
   - Coloca fotos reales en `/images/`
   - Ver lista en `images/placeholder-images.txt`

3. **Configurar FormSpree (formulario):**
   - Ir a formspree.io
   - Crear cuenta gratis
   - Obtener endpoint
   - Actualizar en index.html línea: `<form action="..."`

---

## 🚀 MÉTODO 1: FILE MANAGER (MÁS FÁCIL)

### **PASO 1: Acceder al Panel**

1. Ir al panel de tu hosting:
   - **Hostinger**: hpanel.hostinger.com
   - **cPanel**: tudominio.com/cpanel
   - **SiteGround**: sitetools.siteground.com

2. **Iniciar sesión** con credenciales del email de bienvenida

---

### **PASO 2: Abrir File Manager**

1. Buscar: **"File Manager"** o **"Administrador de Archivos"**
2. Clic para abrir

---

### **PASO 3: Navegar a carpeta web**

Ir a la carpeta raíz del sitio:
- `/public_html/` (más común)
- `/htdocs/`
- `/www/`
- `/html/`

💡 **Esta es la carpeta donde irán tus archivos**

---

### **PASO 4: Limpiar archivos default**

Si hay archivos de ejemplo (index.html, index.php, etc.):
1. Seleccionarlos
2. Clic derecho → **Delete** o **Eliminar**
3. Confirmar

---

### **PASO 5: Subir archivos**

1. **Clic en botón "Upload"** o **"Subir archivos"**

2. **Seleccionar todos los archivos:**
   - index.html
   - README.md
   - .gitignore
   - GITHUB-SETUP.md
   
3. **Esperar que suban** (30 segundos - 2 minutos)

---

### **PASO 6: Subir carpetas**

Subir carpetas una por una:

**Carpeta CSS:**
1. Clic en "Upload"
2. Seleccionar: `css/styles.css`
3. Subir

**Carpeta Images:**
1. Clic en "Upload"
2. Seleccionar todos los archivos de `/images/`
3. Subir (incluyendo logo.png)

---

### **PASO 7: Verificar estructura**

La estructura debe quedar:
```
/public_html/
├── index.html
├── css/
│   └── styles.css
└── images/
    ├── logo.png
    ├── hero-pumps.jpg
    └── ...
```

---

### **PASO 8: Probar el sitio**

1. Abrir navegador
2. Ir a: `http://tudominio.com`
3. Verificar que carga correctamente

---

## 🔐 PASO 9: ACTIVAR SSL (HTTPS)

### **Hostinger:**
1. Panel → SSL → Seleccionar dominio
2. Instalar **Let's Encrypt SSL** (gratis)
3. Esperar 5-10 minutos

### **cPanel:**
1. Buscar **"SSL/TLS Status"**
2. Seleccionar dominio
3. Clic en **"Install SSL"**

### **SiteGround:**
1. Site Tools → Security → SSL Manager
2. Seleccionar dominio
3. **Install** Let's Encrypt

---

### **FORZAR HTTPS:**

1. En File Manager, crear archivo: `.htaccess`
2. Editar y agregar:
```apache
RewriteEngine On
RewriteCond %{HTTPS} off
RewriteRule ^(.*)$ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301]
```
3. Guardar

---

## 📁 MÉTODO 2: FTP CON FILEZILLA

### **PASO 1: Instalar FileZilla**

1. Descargar: https://filezilla-project.org
2. Instalar (siguiente, siguiente...)
3. Abrir FileZilla

---

### **PASO 2: Obtener credenciales FTP**

En tu panel de hosting busca:
- **"FTP Accounts"** o **"Cuentas FTP"**

Anotar:
```
Host: ftp.tudominio.com (o IP)
Usuario: usuario_ftp
Contraseña: tu_contraseña
Puerto: 21
```

---

### **PASO 3: Conectar con FileZilla**

1. En FileZilla, arriba:
   - **Host**: ftp.tudominio.com
   - **Username**: usuario_ftp
   - **Password**: tu_contraseña
   - **Port**: 21

2. Clic en **"Quickconnect"**

3. Si aparece advertencia de certificado → **"OK"**

---

### **PASO 4: Navegar a carpeta web**

**Panel derecho** (servidor):
- Buscar carpeta: `/public_html/`
- Doble clic para entrar

---

### **PASO 5: Subir archivos**

**Panel izquierdo** (tu PC):
- Navegar a carpeta del proyecto

**Subir:**
1. Seleccionar todos los archivos y carpetas
2. Arrastrar al panel derecho
3. Esperar transferencia

---

### **PASO 6: Verificar permisos**

Clic derecho en archivos → **File permissions**
- Archivos: `644` o `755`
- Carpetas: `755`

---

## ✅ VERIFICACIÓN FINAL

### **Checklist:**

- [ ] Sitio carga: `https://tudominio.com` ✅
- [ ] SSL activo (candado en navegador) 🔒
- [ ] Logo visible en navbar
- [ ] Imágenes cargando correctamente
- [ ] Botones WhatsApp funcionan
- [ ] Formulario envía (si configuraste FormSpree)
- [ ] Responsive en móvil
- [ ] Sin errores 404

---

## 🧪 PRUEBAS

### **1. Prueba de velocidad:**
- https://pagespeed.web.dev
- Objetivo: > 80/100

### **2. Prueba responsive:**
- Abrir en celular
- Probar en Chrome DevTools (F12 → Toggle device)

### **3. Prueba de formulario:**
- Completar y enviar
- Verificar email recibido

### **4. Prueba de WhatsApp:**
- Clic en botones
- Verificar que abre WhatsApp
- Verificar mensaje prellenado

---

## 🔧 CONFIGURACIONES ADICIONALES

### **Configurar emails corporativos:**

1. Panel → **"Email Accounts"**
2. Crear: `info@tudominio.com`
3. Configurar en Gmail/Outlook

**Datos típicos:**
```
IMAP:
Host: mail.tudominio.com
Puerto: 993
SSL: Sí

SMTP:
Host: mail.tudominio.com
Puerto: 465
SSL: Sí
```

---

## 🚨 PROBLEMAS COMUNES

### **"Error 500"**
- Revisar permisos de archivos
- Verificar .htaccess
- Ver error_log en File Manager

### **"Error 404"**
- Verificar que index.html existe
- Verificar mayúsculas/minúsculas en nombres

### **CSS no carga**
- Verificar ruta en index.html
- Verificar que /css/styles.css existe
- Limpiar caché: Ctrl+F5

### **Imágenes no cargan**
- Verificar rutas en index.html
- Verificar nombres de archivos
- Comprimir si son muy pesadas (> 1MB)

### **WhatsApp no abre**
- Verificar número: `51948579939`
- Sin espacios ni caracteres especiales
- Probar en móvil real

---

## 📊 OPTIMIZACIONES POST-LANZAMIENTO

### **1. Comprimir imágenes:**
- TinyPNG.com
- Objetivo: < 200KB cada una

### **2. Activar CDN:**
- Cloudflare (gratis)
- Mejora velocidad global

### **3. Caché del navegador:**
Agregar a .htaccess:
```apache
<IfModule mod_expires.c>
  ExpiresActive On
  ExpiresByType image/jpg "access plus 1 year"
  ExpiresByType image/jpeg "access plus 1 year"
  ExpiresByType image/png "access plus 1 year"
  ExpiresByType text/css "access plus 1 month"
  ExpiresByType application/javascript "access plus 1 month"
</IfModule>
```

### **4. Instalar Google Analytics:**
- Crear propiedad en analytics.google.com
- Copiar código
- Pegar antes de `</head>` en index.html

---

## 📱 ACTUALIZACIONES FUTURAS

Para actualizar el sitio:

1. **Editar archivos localmente**
2. **Subir archivos modificados** vía FTP o File Manager
3. **Limpiar caché** del navegador (Ctrl+F5)
4. **Verificar cambios** en el sitio

---

## 💰 COSTOS MENSUALES TÍPICOS

| Servicio | Costo |
|----------|-------|
| Hosting | S/ 15-50/mes |
| Dominio | S/ 45/año |
| SSL | Gratis (Let's Encrypt) |
| FormSpree | Gratis (50 envíos/mes) |
| **TOTAL** | **~S/ 20/mes** |

---

## 📞 SOPORTE

**Hosting:**
- Hostinger: Chat 24/7
- SiteGround: Tickets
- cPanel: Documentación en cpanel.net

**Proyecto:**
- WhatsApp: +51 948 579 939
- Email: comercial@ingdelca.com

---

## ✨ MEJORAS OPCIONALES

Después del lanzamiento:

- [ ] Google Search Console
- [ ] Facebook Pixel
- [ ] Chatbot (Tidio, Tawk.to)
- [ ] Blog WordPress (subdominio)
- [ ] Certificado EV SSL (más caro, más seguro)

---

## 🎉 ¡FELICITACIONES!

Tu landing page está ONLINE y lista para generar leads.

**Próximos pasos:**
1. Compartir en redes sociales
2. Agregar a Google My Business
3. Enviar a clientes
4. Configurar Google Ads (opcional)

---

**¡Éxito con INGDELCA! 🚀**
