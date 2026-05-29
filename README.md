[README.md](https://github.com/user-attachments/files/28411656/README.md)
# color.grade

**→ [Abrir la app](https://jose199201.github.io/ColorMatch-LUT/)**

Herramienta de calibración de color en el navegador. Sube una imagen que quieres editar y otra de referencia, y la app transfiere la paleta de color automáticamente. Sin instalación, sin servidor — todo corre localmente en tu navegador.

---

## Qué hace

- Analiza la distribución de color (media + desviación estándar por canal RGB) de ambas imágenes
- Transfiere la paleta de la referencia a la imagen a editar usando el método Reinhard con soft-clamp para preservar las altas luces
- Permite ajustar intensidad, brillo, contraste y saturación en tiempo real
- Exporta un **LUT 3D de 33×33×33 en formato `.cube`** compatible con Photoshop, Lightroom, DaVinci Resolve y Premiere Pro
- Muestra histogramas comparativos y delta de color por canal

## Cómo usar el LUT en Photoshop

1. Exporta el `.cube` desde la app
2. `Capa → Nueva capa de ajuste → Búsqueda de color`
3. En el panel de propiedades: `Cargar LUT 3D...` → selecciona el `.cube`

## Formatos soportados

Entrada: JPG · PNG · WebP  
Exportación LUT: `.cube` (3D LUT estándar)  
Exportación imagen: PNG

## Privacidad

Ninguna imagen sale de tu navegador. No hay backend, no hay servidor, no hay tracking.

---

Made with vanilla HTML + Canvas API
