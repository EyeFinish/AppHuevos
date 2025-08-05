# 🥚 Página Web para Pedidos de Huevos

Una página web simple y elegante que permite a los clientes hacer pedidos de huevos directamente a través de WhatsApp.

## ✨ Características

- **Diseño moderno y responsivo** - Se adapta a móviles y computadoras
- **Opciones predefinidas de cantidad** - 12, 20, 30 huevos con opción "Otros"
- **Integración con Google Maps** - Selección exacta de ubicación con mapa interactivo
- **Autocompletado de direcciones** - Búsqueda inteligente de ubicaciones
- **Integración directa con WhatsApp** - Se abre automáticamente con el mensaje prellenado
- **Sin backend requerido** - Todo funciona en el frontend
- **Validación de datos** - Asegura que los campos estén completos

## 🚀 Cómo usar

1. **Abrir el archivo** `index.html` en cualquier navegador web
2. **Completar el formulario** con los datos del cliente
3. **Hacer clic en "Pedir por WhatsApp"**
4. **WhatsApp se abrirá automáticamente** con el mensaje listo para enviar

## ⚙️ Personalización

### Configuración del mapa

La página utiliza **OpenStreetMap** con Leaflet, que es completamente gratuito y no requiere API key. El mapa incluye:

- **Búsqueda de direcciones**: Escribe una dirección y presiona Enter
- **Selección manual**: Haz clic en el mapa para seleccionar ubicación
- **Marcador arrastrable**: Mueve el marcador para ajustar la posición
- **Coordenadas exactas**: Se obtienen automáticamente latitud y longitud

### Cambiar el número de WhatsApp

En el archivo `index.html`, busca esta línea:

```javascript
const numeroWhatsApp = "56912345678"; // Cambia este número
```

Reemplaza `56912345678` con el número de la empresa vendedora en formato:
- Código de país (56 para Chile)
- Número sin espacios ni guiones

**Ejemplo:** `56987654321`

### Personalizar el mensaje

Puedes modificar el formato del mensaje en esta sección:

```javascript
const mensaje = `Hola! Soy ${nombre}. 

Quiero hacer un pedido de ${cantidad} huevos.

📍 Mi ubicación es: ${ubicacion}

💰 Pago en efectivo al momento de la entrega.

¡Gracias! 🥚`;
```

### Cambiar el diseño

El CSS está incluido en el mismo archivo. Puedes modificar:
- Colores del gradiente de fondo
- Estilo del formulario
- Tipografía
- Animaciones

## 📱 Funcionamiento en móviles

- En móviles, se abrirá la app de WhatsApp
- En computadoras, se abrirá WhatsApp Web
- El formulario es completamente responsivo

## 🌐 Subir a internet

Para que otros puedan acceder a tu página:

1. **Netlify**: Arrastra la carpeta a netlify.com
2. **Vercel**: Conecta tu repositorio de GitHub
3. **GitHub Pages**: Sube a un repositorio y activa GitHub Pages

## 📋 Campos del formulario

- **Nombre completo**: Nombre del cliente
- **Cantidad de huevos**: Opciones predefinidas (12, 20, 30) o cantidad personalizada
- **Ubicación**: Selección exacta mediante Google Maps con autocompletado de direcciones

## 🔧 Tecnologías utilizadas

- HTML5
- CSS3 (con gradientes y animaciones)
- JavaScript vanilla
- Leaflet.js (mapas interactivos)
- OpenStreetMap (mapas gratuitos)
- Nominatim (geocodificación)
- API de WhatsApp (wa.me)

## 📞 Soporte

Si necesitas ayuda para personalizar la página, puedes:
- Modificar el número de WhatsApp
- Cambiar los colores y estilos
- Agregar campos adicionales al formulario
- Personalizar el mensaje que se envía

---

**¡Listo para usar!** 🎉 