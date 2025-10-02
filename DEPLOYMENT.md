# 🚀 Guía de Despliegue - Portfolio Angel Hidalgo

## 📋 Opciones de Despliegue

### 1. GitHub Pages (Recomendado - Gratis)

#### Paso a paso:
1. **Crear repositorio en GitHub**
   ```bash
   # Inicializar git en el proyecto
   git init
   git add .
   git commit -m "Initial commit: Angel Hidalgo Portfolio"
   
   # Conectar con GitHub (reemplaza con tu usuario)
   git remote add origin https://github.com/[tu-usuario]/angel-hidalgo-portfolio.git
   git branch -M main
   git push -u origin main
   ```

2. **Configurar GitHub Pages**
   - Ve a Settings > Pages en tu repositorio
   - Source: "Deploy from a branch"
   - Branch: "main"
   - Folder: "/ (root)"
   - Guarda los cambios

3. **Acceder a tu página**
   - URL: `https://[tu-usuario].github.io/angel-hidalgo-portfolio`
   - El despliegue toma 1-5 minutos

#### Ventajas:
✅ Completamente gratis
✅ SSL automático (HTTPS)
✅ Fácil de mantener
✅ Dominio personalizado disponible

### 2. Netlify (Fácil y Potente)

#### Opción A - Desde GitHub:
1. Ve a [netlify.com](https://netlify.com)
2. "New site from Git"
3. Conecta tu repositorio de GitHub
4. Deploy automático en cada push

#### Opción B - Drag & Drop:
1. Comprimir todos los archivos en un ZIP
2. Arrastrar el ZIP a netlify.com/drop
3. ¡Listo! URL instantánea

#### Ventajas:
✅ Deploy automático
✅ Dominio personalizado gratis
✅ SSL automático
✅ Formularios funcionales
✅ CDN global

### 3. Vercel (Para Desarrolladores)

```bash
# Instalar Vercel CLI
npm i -g vercel

# Deploy
vercel

# Seguir las instrucciones
```

#### Ventajas:
✅ Deploy súper rápido
✅ Excelente performance
✅ Dominio personalizado
✅ Analytics incluidos

### 4. Firebase Hosting

```bash
# Instalar Firebase CLI
npm install -g firebase-tools

# Login
firebase login

# Inicializar
firebase init hosting

# Deploy
firebase deploy
```

### 5. Hosting Tradicional (cPanel/FTP)

1. **Comprimir archivos**
   - Selecciona todos los archivos del proyecto
   - Crea un archivo ZIP

2. **Subir por FTP**
   - Conecta a tu hosting via FTP
   - Sube todos los archivos a `public_html/` o `/www/`

3. **Configurar dominio**
   - Apunta tu dominio a la carpeta correcta

## 🔧 Configuración de Dominio Personalizado

### Para GitHub Pages:
1. Compra un dominio (ej: angelohidalgo.com)
2. En tu repositorio: Settings > Pages > Custom domain
3. Configura DNS en tu proveedor:
   ```
   Tipo: CNAME
   Nombre: www
   Valor: [tu-usuario].github.io
   
   Tipo: A
   Nombre: @
   Valor: 185.199.108.153
   Valor: 185.199.109.153
   Valor: 185.199.110.153
   Valor: 185.199.111.153
   ```

### Para Netlify:
1. En Netlify: Site settings > Domain management
2. Add custom domain
3. Seguir instrucciones DNS

## 📧 Configuración del Formulario de Contacto

### Netlify Forms (Recomendado):
```html
<!-- Añadir atributo netlify al form -->
<form netlify>
```

### Formspree:
1. Registrarse en formspree.io
2. Cambiar action del form:
```html
<form action="https://formspree.io/f/[tu-id]" method="POST">
```

### EmailJS:
1. Configurar cuenta en emailjs.com
2. Añadir script en HTML
3. Configurar JavaScript

## 🔍 SEO y Analytics

### Google Analytics:
```html
<!-- Añadir antes de </head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

### Google Search Console:
1. Verificar propiedad del sitio
2. Enviar sitemap.xml
3. Monitorear indexación

## 🚀 Optimizaciones Post-Deploy

### 1. Performance:
- Comprimir imágenes
- Minificar CSS/JS
- Configurar cache headers

### 2. SEO:
- Sitemap.xml
- robots.txt
- Meta tags Open Graph

### 3. Monitoreo:
- Google Analytics
- PageSpeed Insights
- Search Console

## 📱 Pruebas Pre-Deploy

### Checklist:
- [ ] Navegación funciona en móvil
- [ ] Formulario envía correctamente
- [ ] Imágenes cargan bien
- [ ] Links funcionan
- [ ] Responsive en todos los tamaños
- [ ] Velocidad aceptable (< 3 segundos)
- [ ] SEO básico configurado

### Herramientas de Testing:
- [PageSpeed Insights](https://pagespeed.web.dev)
- [Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)
- [Lighthouse](https://developers.google.com/web/tools/lighthouse)

## 🔄 Mantenimiento

### Actualizaciones Regulares:
- Actualizar información de proyectos
- Añadir nuevas experiencias
- Actualizar skills y tecnologías
- Revisar links rotos
- Actualizar certificaciones

### Backup:
- Mantener copia en GitHub
- Backup regular de configuraciones
- Documentar cambios importantes

---

## 📞 Soporte

Si necesitas ayuda con el despliegue:
1. Revisa la documentación oficial de cada plataforma
2. Consulta los logs de error
3. Verifica configuraciones DNS (24-48 horas para propagarse)

**¡Tu portfolio profesional estará online en minutos! 🚀**