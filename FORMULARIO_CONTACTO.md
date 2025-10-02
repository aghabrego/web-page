# 📧 CONFIGURACIÓN DEL FORMULARIO DE CONTACTO

## 🚀 **Opción 1: Formspree (RECOMENDADA para GitHub Pages)**

### ✅ **Ventajas:**
- ✅ Funciona con GitHub Pages
- ✅ Gratis hasta 50 envíos/mes
- ✅ Setup súper fácil
- ✅ Spam protection incluido
- ✅ Notificaciones por email

### 📋 **Configuración paso a paso:**

1. **Crear cuenta en Formspree:**
   - Ve a: https://formspree.io
   - Clic en "Get Started"
   - Regístrate con tu email

2. **Crear nuevo formulario:**
   - Clic en "New Form"
   - Nombre: "Angel Hidalgo Portfolio Contact"
   - Email de notificación: tu email personal

3. **Copiar el endpoint:**
   - Te darán una URL como: `https://formspree.io/f/xxxxxx`
   - Reemplaza en el HTML la URL actual

4. **¡Listo!** - El formulario ya funciona

### 🔧 **Configuración actual (ya aplicada):**
```html
<form action="https://formspree.io/f/xdkobpwa" method="POST">
```

---

## 🚀 **Opción 2: EmailJS (Funciona 100% en frontend)**

### ✅ **Ventajas:**
- ✅ Funciona con GitHub Pages
- ✅ No necesita backend
- ✅ Gratis hasta 200 emails/mes
- ✅ Personalizable al 100%

### 📋 **Setup EmailJS:**

1. **Cuenta EmailJS:**
   - Ve a: https://emailjs.com
   - Crear cuenta gratis

2. **Configurar servicio de email:**
   - Add Email Service
   - Conectar Gmail/Outlook
   - Obtener Service ID

3. **Crear template:**
   - Email Templates → Create New Template
   - Diseñar el email que recibirás
   - Obtener Template ID

4. **Código JavaScript:**
```javascript
// Agregar al HTML antes de </head>
<script src="https://cdn.emailjs.com/dist/email.min.js"></script>

// En script.js
emailjs.init("TU_USER_ID");

// En el form submit:
emailjs.send("TU_SERVICE_ID", "TU_TEMPLATE_ID", {
    name: name,
    email: email,
    subject: subject,
    message: message
});
```

---

## 🚀 **Opción 3: Netlify Forms (Si cambias a Netlify)**

### ✅ **Ventajas:**
- ✅ Súper fácil (solo agregar atributo)
- ✅ Spam protection automático
- ✅ Dashboard para ver envíos
- ✅ Notificaciones automáticas

### 📋 **Setup Netlify:**

1. **Subir a Netlify:**
   - Ve a: https://netlify.com
   - Drag & drop tu carpeta de proyecto
   - O conectar con GitHub

2. **Activar formularios:**
```html
<form netlify>
  <!-- Solo agregar el atributo netlify -->
</form>
```

3. **¡Automático!** - Netlify detecta y configura todo

---

## 🚀 **Opción 4: Google Forms (Súper simple)**

### ✅ **Ventajas:**
- ✅ Completamente gratis
- ✅ Integración con Google Sheets
- ✅ Sin configuración complicada

### 📋 **Setup Google Forms:**

1. **Crear Google Form:**
   - Ve a: https://forms.google.com
   - Crear formulario con campos: Nombre, Email, Asunto, Mensaje

2. **Obtener URL del form:**
   - Clic en "Enviar" → Enlace
   - Copiar URL

3. **Cambiar action del form:**
```html
<form action="TU_GOOGLE_FORM_URL" target="_blank">
```

---

## 🚀 **Opción 5: Backend Propio (Avanzado)**

### 🔧 **Para desarrolladores:**

#### **Node.js + Express:**
```javascript
const express = require('express');
const nodemailer = require('nodemailer');
const app = express();

app.post('/contact', async (req, res) => {
    // Configurar nodemailer
    // Enviar email
    // Responder al frontend
});
```

#### **PHP (Hosting tradicional):**
```php
<?php
if ($_POST) {
    $name = $_POST['name'];
    $email = $_POST['email'];
    $subject = $_POST['subject'];
    $message = $_POST['message'];
    
    // Validar datos
    // Enviar email con mail()
    // Responder JSON
}
?>
```

---

## 🎯 **RECOMENDACIÓN PARA TU CASO:**

### Para GitHub Pages: **Formspree** ⭐
- Fácil configuración
- Funciona inmediatamente
- Plan gratuito suficiente

### Para máximo control: **EmailJS** ⭐
- 100% frontend
- Muy personalizable
- Mejor UX

---

## 📱 **Configuración de Notificaciones**

### **Email que recibirás:**
```
De: Formulario Portfolio Angel Hidalgo
Asunto: Nuevo contacto: [ASUNTO]

Nombre: [NOMBRE]
Email: [EMAIL]
Asunto: [ASUNTO]

Mensaje:
[MENSAJE]

---
Enviado desde: angelohidalgo.com
Fecha: [FECHA/HORA]
```

### **Respuesta automática al visitante:**
```
¡Gracias por contactarme!

Hola [NOMBRE],

He recibido tu mensaje y te responderé en las próximas 24 horas.

Saludos,
Angel Hidalgo
CTO - Weirdo Labs
```

---

## ⚡ **IMPLEMENTACIÓN RÁPIDA:**

### **Para activar YA (recomendado):**

1. **Ir a Formspree.io**
2. **Crear cuenta gratis**
3. **Crear formulario**
4. **Reemplazar URL en el HTML**
5. **Commit y push a GitHub**
6. **¡Formulario funcionando!**

### **Tiempo total: 5 minutos** ⏱️

¿Quieres que configure alguna opción específica o prefieres que te ayude con Formspree que es la más directa?