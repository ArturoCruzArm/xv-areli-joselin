# Guía: Publicar Invitación en GitHub Pages usando GitHub CLI

## 📋 Prerrequisitos

1. Tener Git instalado
2. Tener GitHub CLI (gh) instalado
3. Estar autenticado en GitHub CLI

## 🔐 Autenticación en GitHub CLI

Si es la primera vez usando GitHub CLI:

```bash
gh auth login
```

Sigue las instrucciones:
- Selecciona "GitHub.com"
- Selecciona "HTTPS"
- Autentícate con tu navegador o token

## 🚀 Pasos para Publicar

### 1. Inicializar Repositorio Git

```bash
cd C:\Users\foro7\xv-anos-dulce-camila
git init
git add .
git commit -m "Initial commit: XV años Dulce Camila Aviña Franco"
```

### 2. Crear Repositorio en GitHub

```bash
gh repo create xv-anos-dulce-camila --public --source=. --remote=origin --description "Invitación web para los XV años de Dulce Camila - 16 Mayo 2026"
```

### 3. Subir Archivos a GitHub

```bash
git push -u origin main
```

### 4. Habilitar GitHub Pages

```bash
gh repo edit --enable-pages --pages-branch main
```

O manualmente:
1. Ve a https://github.com/[tu-usuario]/xv-anos-dulce-camila
2. Click en "Settings"
3. Click en "Pages" en el menú lateral
4. En "Source" selecciona "main" branch
5. Click "Save"

### 5. Obtener la URL

```bash
gh repo view --web
```

La URL será: `https://[tu-usuario].github.io/xv-anos-dulce-camila/`

## 🔄 Actualizar la Invitación

Cada vez que hagas cambios:

```bash
# Ver cambios
git status

# Agregar cambios
git add .

# Hacer commit
git commit -m "Descripción de los cambios"

# Subir a GitHub
git push
```

Los cambios se reflejarán en la web en 1-2 minutos.

## 📝 Comandos Útiles

### Ver estado del repositorio
```bash
git status
```

### Ver historial de commits
```bash
git log --oneline
```

### Ver repositorio en navegador
```bash
gh repo view --web
```

### Ver la página publicada
```bash
# En Windows
start https://[tu-usuario].github.io/xv-anos-dulce-camila/

# O simplemente abre en tu navegador
```

## 🌐 Dominio Personalizado (Opcional)

### 1. Crear archivo CNAME

```bash
echo "dulcecamila.tudominio.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

### 2. Configurar DNS

En tu proveedor de dominio (GoDaddy, Namecheap, etc.):

**Opción A: Usar subdominio (recomendado)**
- Tipo: CNAME
- Nombre: dulcecamila (o el subdominio que quieras)
- Valor: [tu-usuario].github.io
- TTL: 3600

**Opción B: Usar dominio raíz**
- Tipo: A
- Nombre: @
- Valor: 185.199.108.153
- Agregar más registros A:
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153

### 3. Habilitar HTTPS

En GitHub Pages settings, marca "Enforce HTTPS" (tarda unas horas en activarse).

## 🔧 Solución de Problemas

### Error: "remote origin already exists"
```bash
git remote remove origin
gh repo create xv-anos-dulce-camila --public --source=. --remote=origin
```

### La página no se actualiza
- Espera 1-2 minutos
- Limpia caché del navegador (Ctrl + F5)
- Verifica que el push fue exitoso: `git log`

### Error 404
- Verifica que GitHub Pages esté habilitado
- Asegúrate que el archivo se llame `index.html`
- La URL debe ser exacta (case-sensitive)

## 📱 Compartir la Invitación

Una vez publicada:

### WhatsApp
```
¡Estás invitado/a a los XV años de Dulce Camila! 🎉

📅 16 de Mayo, 2026
⛪ 5:00 PM - Templo de los Laureles

Ver invitación completa:
https://[tu-usuario].github.io/xv-anos-dulce-camila/

¡Confirma tu asistencia! 💕
```

### Facebook/Instagram
```
¡Celebremos juntos! 💜✨

Mis XV Años
Dulce Camila
16.05.2026

Ver detalles e invitación:
[link]

#MisXVAños #DulceCamila #Quinceañera
```

## 🎨 Personalizar Después de Publicar

### Agregar fotos de la sesión:

1. Optimiza las fotos
2. Súbelas a la carpeta `images/`
3. Actualiza `index.html` con las rutas
4. Commit y push

```bash
git add images/
git add index.html
git commit -m "Agregar fotos de sesión previa"
git push
```

### Actualizar información:

1. Edita el archivo correspondiente (index.html, logistica.html, etc.)
2. Guarda los cambios
3. Commit y push

```bash
git add .
git commit -m "Actualizar información del evento"
git push
```

## 📊 Opcional: Google Analytics

Para ver cuántas personas visitan la invitación:

1. Crea cuenta en Google Analytics
2. Obtén el código de seguimiento
3. Agrégalo antes de `</head>` en todos los HTML
4. Commit y push

## 🔒 Privacidad y Seguridad

- No incluyas información bancaria sensible
- No publiques direcciones exactas de casa
- Los números de teléfono pueden ser públicos si estás de acuerdo
- El contrato puede dejarse privado (no linkear desde la invitación principal)

## 💡 Tips

1. **Prueba primero en local:** Abre los archivos HTML en tu navegador antes de publicar
2. **Usa nombres descriptivos en commits:** Facilita encontrar cambios después
3. **Haz respaldos:** GitHub ya es un respaldo, pero guarda copias locales
4. **Actualiza regularmente:** Mantén la información al día

## 📞 Ayuda

Si necesitas ayuda:
- GitHub CLI docs: https://cli.github.com/manual/
- GitHub Pages docs: https://docs.github.com/pages
- Contacta a Foro 7: 477-920-3776

---

*Guía creada por Foro 7 Producciones*
