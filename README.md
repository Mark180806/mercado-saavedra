# Mercado Saavedra Fajardo — Landing Page

Landing page oficial del Mercado Saavedra Fajardo de Murcia.  
Diseñada para móvil (QR), con vale de 150€ y directorio completo de puestos.

---

## 🚀 Instalación y uso

### 1. Instalar dependencias
```bash
npm install
```

### 2. Iniciar servidor
```bash
npm start
```

### 3. Abrir en el navegador
```
http://localhost:3000
```

---

## 📁 Estructura del proyecto

```
mercado-saavedra/
├── server.js              ← Servidor Express (Node.js)
├── package.json
└── public/
    ├── index.html         ← Landing page completa
    ├── uploads/           ← Fotos del ticket (subidas por el usuario)
    └── images/
        ├── gallery/       ← Imágenes de la galería
        └── puestos/       ← Fotos de cada puesto
```

---

## 📸 Cómo añadir fotos

### Foto del exterior / hero
- En la web, toca el botón **"📸 Foto exterior"** (arriba a la derecha en el hero)
- Selecciona la imagen y se mostrará de fondo

### Foto del vale/ticket
- En la sección del Vale 150€, toca la zona central del ticket
- Sube la foto que quieras mostrar en el ticket

### Fotos de los puestos
- En cada tarjeta de puesto, toca la zona **"📷 Añadir foto del puesto"**
- La foto se guarda y se muestra en la tarjeta

### Galería (18 imágenes)
- Haz **doble clic** en cualquier celda de la galería para subir una foto
- Puedes filtrar por categoría con los botones de filtro

---

## 🌐 Despliegue en producción

Para publicar online (por ejemplo en Railway, Render, Fly.io o VPS):

```bash
# Variable de entorno para el puerto
PORT=3000 node server.js
```

O con PM2:
```bash
npm install -g pm2
pm2 start server.js --name mercado-saavedra
pm2 save
```

---

## 📱 Secciones de la web

1. **Hero** — Foto del mercado + horario (Lun-Sáb 8:00-15:00)
2. **Vale 150€** — Ticket con foto subible, condiciones claras
3. **Sobre el mercado** — Descripción y categorías
4. **Puestos** — Directorio interactivo con contacto y foto por puesto
5. **Galería** — 18 imágenes con filtros y lightbox
6. **Ubicación** — Google Maps integrado
7. **Redes sociales** — Instagram y Facebook
8. **Footer**

---

## 🔗 Redes sociales configuradas

- Instagram: https://www.instagram.com/mercado_saavedra_fajardo/
- Facebook: https://www.facebook.com/mercasaavedrafajardo/?locale=es_ES

---

## 📞 Dependencias

- `express` — Servidor web
- `multer` — Gestión de subida de archivos
