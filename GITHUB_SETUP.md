# 🚀 INSTRUCCIONES PARA PUBLICAR EN GITHUB

## 📋 Paso 1: Crear Repositorio en GitHub

1. **Ve a GitHub.com y haz login**
   - Si no tienes cuenta, créala en: https://github.com/join

2. **Crear nuevo repositorio**
   - Clic en el botón "+" (esquina superior derecha)
   - Selecciona "New repository"

3. **Configuración del repositorio:**
   ```
   Repository name: angel-hidalgo-portfolio
   Description: Portfolio profesional de Angel Hidalgo - CTO & Desarrollador de Software
   
   ✅ Public (para que sea visible)
   ❌ Add a README file (ya tenemos uno)
   ❌ Add .gitignore (ya tenemos uno)
   ❌ Choose a license (opcional)
   ```

4. **Clic en "Create repository"**

## 📋 Paso 2: Conectar el Proyecto Local con GitHub

Copia y ejecuta estos comandos en la terminal (REEMPLAZA 'tu-usuario' con tu usuario real de GitHub):

```bash
# Conectar con el repositorio remoto
git remote add origin https://github.com/tu-usuario/angel-hidalgo-portfolio.git

# Subir los archivos a GitHub
git push -u origin main
```

**EJEMPLO** (si tu usuario fuera "angelhidalgo"):
```bash
git remote add origin https://github.com/angelhidalgo/angel-hidalgo-portfolio.git
git push -u origin main
```

## 📋 Paso 3: Activar GitHub Pages

1. **En tu repositorio de GitHub:**
   - Ve a la pestaña "Settings"
   - Scroll hacia abajo hasta "Pages" (menú lateral izquierdo)

2. **Configurar GitHub Pages:**
   ```
   Source: Deploy from a branch
   Branch: main
   Folder: / (root)
   ```

3. **Clic en "Save"**

4. **¡Espera 1-5 minutos!**
   - GitHub procesará los archivos
   - Te dará una URL como: `https://tu-usuario.github.io/angel-hidalgo-portfolio`

## 🌐 Tu Página Estará Disponible En:

```
https://tu-usuario.github.io/angel-hidalgo-portfolio
```

**EJEMPLO:**
```
https://angelhidalgo.github.io/angel-hidalgo-portfolio
```

## 🔧 Comandos para Futuras Actualizaciones

Cuando quieras actualizar la página:

```bash
# Navegar al proyecto
cd /home/weirdolabs/code/weirdolabs/web-page

# Agregar cambios
git add .

# Commit con mensaje
git commit -m "Actualización: descripción de cambios"

# Subir a GitHub
git push origin main
```

## ✅ Verificación

Para verificar que todo está bien:

1. **Repositorio creado**: ✅ Visible en tu perfil de GitHub
2. **Archivos subidos**: ✅ 8 archivos en el repositorio
3. **GitHub Pages activo**: ✅ URL funcionando
4. **Página carga**: ✅ Se ve correctamente

## 🆘 Si Hay Problemas

### Error: Repository not found
- Verifica que el nombre del repositorio sea correcto
- Asegúrate de que el repositorio sea público

### Error: Permission denied
- Verifica tus credenciales de GitHub
- Puede necesitar un Personal Access Token

### Página no carga
- Espera 5-10 minutos después de activar Pages
- Verifica que el archivo se llame exactamente "index.html"

## 🎯 ¡LISTO!

Una vez completados estos pasos, tu portfolio profesional estará disponible públicamente en internet y cualquier persona podrá verlo con la URL de GitHub Pages.

**¡Tu página web profesional estará online! 🚀**