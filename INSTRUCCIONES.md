# INSTRUCCIONES - Repositorio XV Años Dulce Camila

## 📁 Estructura del Proyecto

Este repositorio contiene todo lo necesario para gestionar el evento de XV años de Dulce Camila Aviña Franco:

### Archivos Principales

1. **README.md** - Resumen completo del evento con toda la información
2. **index.html** - Invitación web (página principal)
3. **contrato.html** - Contrato de servicios con Foro 7
4. **logistica.html** - Organización y checklist del evento
5. **publicidad.html** - Catálogo de servicios de Foro 7

### Archivos de Configuración

- **.gitignore** - Archivos a ignorar en Git
- **favicon.svg** - Icono del sitio web
- **README-WEB.md** - Guía sobre la invitación web
- **GUIA-GITHUB-CLI.md** - Guía completa para publicar en GitHub
- **setup-github.bat** - Script para configuración inicial
- **push-to-github.bat** - Script para actualizar la página

### Carpetas

- **css/** - Hojas de estilo (actualmente vacía, estilos en línea)
- **js/** - JavaScript (actualmente vacía)
- **images/** - Fotos del evento (pendiente de sesión)

## 🚀 Primeros Pasos

### Opción 1: Ver Archivos Localmente

1. Abre cualquier archivo .html en tu navegador
2. Navega entre las diferentes páginas
3. Revisa la información del contrato

### Opción 2: Publicar en Internet

**Método Fácil (Recomendado):**

1. Asegúrate de tener Git y GitHub CLI instalados
2. Ejecuta `setup-github.bat` (doble clic)
3. Sigue las instrucciones en pantalla
4. ¡Listo! Tu invitación estará en línea

**Método Manual:**

Ver `GUIA-GITHUB-CLI.md` para instrucciones paso a paso

## ✏️ Personalizar la Invitación

### Información Pendiente

Necesitas solicitar a Ana Leticia Franco Sánchez:

1. **Urgente (para el contrato):**
   - Nombre completo del papá de Dulce Camila
   - Hora exacta de inicio de la fiesta
   - Fecha de sesión fotográfica

2. **Importante (para invitación web):**
   - Código de vestuario
   - Colores de la fiesta
   - Mensaje especial
   - Fotos de la sesión previa

### Cómo Actualizar

1. Abre el archivo correspondiente (.html) en un editor de texto
2. Busca el texto que quieres cambiar
3. Guarda los cambios
4. Si está publicado, ejecuta `push-to-github.bat`

## 📸 Agregar Fotos

Una vez realizada la sesión fotográfica:

1. Selecciona las mejores 5-10 fotos
2. Optimízalas (reduce tamaño si es necesario)
3. Guárdalas en la carpeta `images/`
4. Actualiza `index.html` para mostrarlas en la galería

### Código para agregar fotos a la galería:

En `index.html`, busca la sección "Galería de Fotos" y reemplaza con:

```html
<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 1rem; margin-top: 2rem;">
    <img src="images/foto1.jpg" alt="Dulce Camila" style="width: 100%; border-radius: 10px;">
    <img src="images/foto2.jpg" alt="Dulce Camila" style="width: 100%; border-radius: 10px;">
    <img src="images/foto3.jpg" alt="Dulce Camila" style="width: 100%; border-radius: 10px;">
    <!-- Agregar más fotos según necesites -->
</div>
```

## 🎨 Cambiar Colores

Los colores actuales son morado/púrpura. Para cambiar:

1. Abre cada archivo .html
2. Busca los códigos de color:
   - `#667eea` (morado claro)
   - `#764ba2` (morado oscuro)
3. Reemplázalos con los colores del evento

### Generadores de colores recomendados:
- https://coolors.co/
- https://uigradients.com/

## 📱 Compartir la Invitación

Una vez publicada en GitHub Pages:

### Mensaje sugerido para WhatsApp:

```
✨ ¡Estás invitado/a a mis XV años! ✨

Dulce Camila
16 de Mayo, 2026

⛪ Ceremonia: 5:00 PM
   Templo de los Laureles

🎉 Recepción:
   La Haciendita

Ver invitación completa y confirmar asistencia:
[LINK DE GITHUB PAGES]

¡Te espero! 💜
```

### Código QR (Opcional)

Genera un código QR del link en:
- https://www.qr-code-generator.com/

Úsalo en:
- Invitaciones impresas
- Tarjetas
- Decoración del evento

## 🔄 Actualizaciones Frecuentes

### Antes de la sesión:
- Confirmar fecha y hora
- Actualizar `logistica.html` con la información

### Después de la sesión:
- Subir fotos a `images/`
- Actualizar galería en `index.html`
- Activar selector de fotos para que cliente elija sus favoritas

### Antes del evento:
- Actualizar cuenta regresiva (si la agregas)
- Confirmar detalles finales
- Recordar confirmación de asistencia

### Después del evento:
- Subir fotos destacadas
- Agregar video (si decides incluirlo)
- Mantener como recuerdo digital

## 💰 Pagos Pendientes

**Información Importante:**

- **Total del servicio:** $6,500
- **Apartado pagado:** $500 (20 dic 2025)
- **Saldo pendiente:** $6,000
- **Fecha límite:** 9 de mayo de 2026

**Cuenta BBVA:**
- Número: 4152 3137 6890 8985
- Titular: Juan Arturo Cruz Armenta

## 📋 Checklist Foro 7

### Antes de la sesión:
- [ ] Confirmar fecha con clienta
- [ ] Verificar equipo fotográfico
- [ ] Cargar baterías
- [ ] Formatear tarjetas de memoria

### Antes del evento:
- [ ] Recibir saldo ($6,000)
- [ ] Verificar direcciones
- [ ] Confirmar horarios
- [ ] Preparar equipo completo

### Después del evento:
- [ ] Respaldar material
- [ ] Editar fotografías
- [ ] Editar video
- [ ] Entregar material al cliente

## 🆘 Problemas Comunes

### La página no se ve bien en móvil
- Todos los archivos son responsive
- Prueba en diferentes dispositivos
- Limpia caché del navegador

### No se pueden ver las imágenes
- Verifica que las rutas sean correctas
- Las rutas son relativas: `images/foto.jpg`
- Nombres de archivo no deben tener espacios

### Error al hacer push
- Verifica que estás autenticado: `gh auth status`
- Asegúrate que hiciste commit: `git status`

## 📞 Contacto

**Cliente:**
- Ana Leticia Franco Sánchez
- Tel: 477 668 4807

**Foro 7:**
- WhatsApp: 477-920-3776
- Email: foro7producciones@gmail.com
- Ubicación: Padilla 112, Cumbres de Arbide, León, Gto.

## 💡 Consejos Finales

1. **Haz respaldos regulares** de todos los archivos
2. **Prueba todo antes de compartir** el link público
3. **Mantén comunicación** constante con la clienta
4. **Actualiza la información** conforme la recibas
5. **Documenta todo** en README.md

---

**¡Éxito con el proyecto!**

*Creado por Foro 7 Producciones - Diciembre 2025*
