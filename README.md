# PWA 2025 - Progressive Web Application

Esta es una aplicación web progresiva (PWA) con las siguientes características:
- Service Worker para funcionalidad offline
- Web App Manifest para instalación
- Canvas con funciones de dibujo
- Integración con QuickChart API

## Despliegue en GitHub Pages

Para desplegar esta PWA en GitHub Pages:

1. **Habilitar GitHub Pages:**
   - Ve a la configuración del repositorio en GitHub
   - Navega a "Pages" en el menú izquierdo
   - En "Source", selecciona "GitHub Actions"

2. **Despliegue automático:**
   - El workflow de GitHub Actions se ejecutará automáticamente al hacer push a la rama `main`
   - El sitio estará disponible en: `https://[usuario].github.io/pwa2`

3. **Verificar el despliegue:**
   - Ve a la pestaña "Actions" para monitorear el progreso del despliegue
   - Una vez completado, la PWA estará accesible desde la URL de GitHub Pages

## Estructura del proyecto

- `index.html` - Página principal
- `manifest.json` - Manifiesto de la PWA
- `sw.js` - Service Worker
- `lib1.js` - Librería para gráficos QuickChart
- `lib2.js` - Librería para canvas
- `iconos/` - Iconos de la aplicación
- `.github/workflows/deploy.yml` - Script de despliegue automático

## Uso

La aplicación permite:
- Ver gráficos dinámicos usando parámetros URL (`?n=valor&d=valor`)
- Dibujar líneas en canvas haciendo clic en "Exhibir líneas"
- Funciona offline gracias al Service Worker
