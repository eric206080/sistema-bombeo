# 📦 GUÍA RÁPIDA: SUBIR A GITHUB

## 🎯 Objetivo
Subir tu landing page de INGDELCA a GitHub para control de versiones y despliegue.

---

## 📋 REQUISITOS PREVIOS

1. **Cuenta de GitHub**: Crear en github.com (gratis)
2. **Git instalado**: Descargar en git-scm.com
3. **Archivos del proyecto**: Los que acabas de descargar

---

## 🚀 PASO A PASO

### **PASO 1: Crear repositorio en GitHub**

1. Ve a: https://github.com
2. Clic en **"+"** arriba derecha → **"New repository"**
3. Configurar:
   - **Repository name**: `ingdelca-landing`
   - **Description**: `Landing page profesional de INGDELCA - Soluciones de Bombeo Industrial`
   - **Public** o **Private** (tu elección)
   - ✅ **NO** marcar "Add a README file" (ya lo tienes)
   - Clic en **"Create repository"**

4. **Guardar la URL** que aparece (ejemplo):
   ```
   https://github.com/TU-USUARIO/ingdelca-landing.git
   ```

---

### **PASO 2: Preparar archivos localmente**

1. **Abrir terminal/CMD** en la carpeta del proyecto:
   ```bash
   cd /ruta/a/ingdelca-project
   ```

2. **Inicializar Git:**
   ```bash
   git init
   ```

3. **Agregar todos los archivos:**
   ```bash
   git add .
   ```

4. **Hacer primer commit:**
   ```bash
   git commit -m "Initial commit: Landing page INGDELCA"
   ```

5. **Configurar rama principal:**
   ```bash
   git branch -M main
   ```

6. **Conectar con GitHub** (usar tu URL del paso 1):
   ```bash
   git remote add origin https://github.com/TU-USUARIO/ingdelca-landing.git
   ```

7. **Subir archivos:**
   ```bash
   git push -u origin main
   ```

8. **Si pide credenciales:**
   - Usuario: Tu username de GitHub
   - Contraseña: Necesitas un **Personal Access Token** (ver abajo)

---

### **PASO 3: Crear Personal Access Token (si es necesario)**

1. Ve a: GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Clic en **"Generate new token"** → **"Generate new token (classic)"**
3. Configurar:
   - **Note**: "INGDELCA Landing Push"
   - **Expiration**: 90 days (o más)
   - ✅ Marcar: **repo** (todos los sub-permisos)
4. Clic en **"Generate token"**
5. **COPIAR Y GUARDAR** el token (no se volverá a mostrar)
6. Usar este token como contraseña al hacer `git push`

---

### **PASO 4: Verificar en GitHub**

1. Ve a tu repositorio: `https://github.com/TU-USUARIO/ingdelca-landing`
2. Deberías ver todos tus archivos
3. El README.md se mostrará automáticamente

---

## 🌐 PASO 5 (OPCIONAL): Activar GitHub Pages

**¡Hostea tu sitio GRATIS en GitHub!**

1. En tu repositorio, ve a: **Settings** → **Pages**
2. En **"Source"**:
   - **Deploy from a branch**
   - **Branch**: `main`
   - **Folder**: `/ (root)`
3. Clic en **"Save"**
4. Espera 2-3 minutos
5. Tu sitio estará en:
   ```
   https://TU-USUARIO.github.io/ingdelca-landing/
   ```

---

## 🔄 ACTUALIZACIONES FUTURAS

Cada vez que hagas cambios:

```bash
# 1. Guardar cambios
git add .

# 2. Hacer commit con mensaje descriptivo
git commit -m "Actualización: agregadas imágenes reales"

# 3. Subir a GitHub
git push
```

---

## 💡 COMANDOS ÚTILES

```bash
# Ver estado de archivos
git status

# Ver historial de commits
git log

# Crear nueva rama
git checkout -b nueva-rama

# Cambiar de rama
git checkout main

# Ver remotes configurados
git remote -v

# Descargar cambios (si trabajas en equipo)
git pull
```

---

## 🚨 PROBLEMAS COMUNES

### **Error: "Permission denied"**
**Solución:** Usar Personal Access Token como contraseña

### **Error: "Repository not found"**
**Solución:** Verificar URL del repositorio con `git remote -v`

### **No pide credenciales (Windows)**
**Solución:** 
```bash
git config --global credential.helper wincred
```

### **Quiero cambiar la URL del repositorio**
```bash
git remote set-url origin https://github.com/NUEVA-URL.git
```

---

## 📊 ESTRUCTURA EN GITHUB

```
ingdelca-landing/
├── .gitignore
├── README.md
├── index.html
├── css/
│   └── styles.css
├── images/
│   ├── logo.png
│   └── placeholder-images.txt
└── js/
    └── (vacío)
```

---

## ✅ CHECKLIST FINAL

- [ ] Repositorio creado en GitHub
- [ ] Git inicializado localmente
- [ ] Archivos subidos con `git push`
- [ ] README.md visible en GitHub
- [ ] Logo visible en repositorio
- [ ] (Opcional) GitHub Pages activado
- [ ] URL pública funcionando

---

## 🎉 ¡LISTO!

Tu proyecto está en GitHub y listo para:
- ✅ Control de versiones
- ✅ Colaboración
- ✅ Backup automático
- ✅ Despliegue gratuito (con Pages)

---

## 📞 ¿NECESITAS AYUDA?

- 📚 Docs Git: git-scm.com/doc
- 📚 Docs GitHub: docs.github.com
- 💬 WhatsApp: +51 948 579 939
- 📧 Email: comercial@ingdelca.com

---

**¡Éxito con tu landing page! 🚀**
