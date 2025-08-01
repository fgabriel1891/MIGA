# 🗺️ Mapa Interactivo Ecuador

Una aplicación web moderna e interactiva para visualizar mapas de Ecuador con información de zonas de envío y costos de entrega.

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![PWA](https://img.shields.io/badge/PWA-ready-purple.svg)

## ✨ Características

### 🎨 Interfaz Moderna
- **Diseño responsivo** que se adapta a todos los dispositivos
- **Tema claro/oscuro** con persistencia en localStorage
- **Tipografía profesional** usando Inter font
- **Iconografía consistente** con Font Awesome
- **Animaciones fluidas** con transiciones CSS

### 🗺️ Funcionalidades del Mapa
- **Múltiples capas de mapas**: OpenStreetMap, Vista satélite, Terreno
- **Geolocalización** para encontrar tu ubicación actual
- **Búsqueda de ubicaciones** con autocompletado
- **Controles de zoom** personalizados
- **Escala métrica** para referencia de distancias
- **Pantalla completa** para mejor visualización

### 📍 Zonas de Entrega
- **Visualización de zonas** con marcadores coloridos
- **Información de precios** por zona de entrega
- **Leyenda interactiva** para referencia rápida
- **Popups informativos** con detalles de cada zona

### 🚀 Progressive Web App (PWA)
- **Instalable** como aplicación nativa
- **Funciona offline** con Service Worker
- **Cacheo inteligente** de recursos
- **Iconos optimizados** para todas las plataformas
- **Atajos de aplicación** para acceso rápido

### ♿ Accesibilidad
- **Navegación por teclado** completa
- **Etiquetas ARIA** apropiadas
- **Contraste optimizado** para legibilidad
- **Soporte para lectores de pantalla**
- **Indicadores de foco** visibles

## 🛠️ Tecnologías Utilizadas

- **HTML5** - Estructura semántica moderna
- **CSS3** - Estilos avanzados con CSS Custom Properties
- **JavaScript ES6+** - Programación moderna con clases
- **Leaflet.js** - Biblioteca de mapas interactivos
- **OpenStreetMap** - Datos de mapas libres
- **Service Worker** - Funcionalidad offline
- **Web App Manifest** - Configuración PWA

## 🚀 Inicio Rápido

1. **Clona o descarga** el repositorio
2. **Abre** `index.html` en tu navegador moderno
3. **¡Disfruta!** del mapa interactivo

### Instalación como PWA

1. Abre la aplicación en tu navegador
2. Busca el ícono de "Instalar" en la barra de direcciones
3. Sigue las instrucciones para instalar en tu dispositivo

## 📱 Uso

### Navegación Básica
- **Zoom**: Usa los controles + / - o la rueda del ratón
- **Panorámica**: Arrastra el mapa con el ratón o toca y arrastra en móvil
- **Capas**: Usa el control de capas en la esquina superior derecha

### Funciones Avanzadas
- **🎯 Mi Ubicación**: Haz clic en el botón de ubicación para centrarte en tu posición
- **🔍 Búsqueda**: Escribe una dirección o lugar en la barra de búsqueda
- **🌙 Tema**: Alterna entre modo claro y oscuro con el botón de tema
- **📺 Pantalla Completa**: Expande a pantalla completa para mejor experiencia

### Zonas de Entrega

El mapa muestra 4 zonas principales de entrega:

| Zona | Color | Precio |
|------|--------|--------|
| Norte | 🟢 Verde | $3.00 |
| Centro | 🔵 Azul | $2.50 |
| Sur | 🟡 Amarillo | $3.50 |
| Valle | 🔴 Rojo | $4.00 |

## 🎨 Personalización

### Cambiar Colores
Modifica las variables CSS en `:root` para personalizar la paleta de colores:

```css
:root {
    --primary-color: #2563eb;
    --primary-dark: #1d4ed8;
    /* ... más variables */
}
```

### Agregar Nuevas Zonas
Modifica el array `deliveryZones` en el JavaScript:

```javascript
const deliveryZones = [
    {
        name: "Nueva Zona",
        coords: [-0.XX, -78.XX],
        price: "$X.XX",
        color: "#hexcolor"
    }
    // ... más zonas
];
```

### Cambiar Capas de Mapa
Agrega nuevas capas en `baseLayers`:

```javascript
const baseLayers = {
    "Nueva Capa": L.tileLayer('https://...', {
        attribution: '...',
        maxZoom: 19
    })
};
```

## 📂 Estructura del Proyecto

```
mapa-ecuador/
├── index.html          # Aplicación principal
├── manifest.json       # Configuración PWA
├── sw.js              # Service Worker
├── README.md          # Documentación
└── mapa.html          # Archivo original (legacy)
```

## 🌐 Compatibilidad

### Navegadores Soportados
- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

### Dispositivos
- ✅ Desktop (Windows, macOS, Linux)
- ✅ Tablets (iOS, Android)
- ✅ Móviles (iOS, Android)

## 🔧 Configuración Avanzada

### Variables de Entorno
La aplicación no requiere variables de entorno específicas, pero puedes configurar:

- **Límites geográficos**: Modifica las coordenadas en el código
- **Zoom por defecto**: Cambia el valor inicial del zoom
- **Centro del mapa**: Ajusta las coordenadas iniciales

### Servicios Externos
- **Nominatim**: Para búsqueda de ubicaciones (no requiere API key)
- **OpenStreetMap**: Para tiles de mapa (gratuito)
- **ArcGIS**: Para vista satelital (gratuito con límites)

## 🤝 Contribución

¡Las contribuciones son bienvenidas! Para contribuir:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - mira el archivo [LICENSE](LICENSE) para detalles.

## 🙏 Reconocimientos

- **Leaflet** - Biblioteca de mapas JavaScript
- **OpenStreetMap** - Datos de mapas abiertos
- **Font Awesome** - Iconografía
- **Inter Font** - Tipografía moderna
- **Nominatim** - Servicio de geocodificación

## 📞 Soporte

¿Problemas o preguntas? 

- 📧 Crea un [issue](https://github.com/tu-usuario/mapa-ecuador/issues)
- 💬 Contacta al equipo de desarrollo

---

**Hecho con ❤️ para Ecuador** 🇪🇨