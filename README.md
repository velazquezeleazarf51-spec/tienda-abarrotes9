# Abarrotes POS - Sistema de Inventario y Ventas con Códigos de Barras

Aplicación web completa para tiendas de abarrotes, minisúper, papelerías, joyerías, deportes y negocios similares.

## Características

- **Inventario**: Agregar, editar, eliminar productos con **descripción**, categorías, unidades, precio de costo, precio de venta y stock (soporta decimales).
- **Códigos de barras**: Generar, descargar e imprimir (individual o varios a la vez). Incluye nombre, descripción y precio en la etiqueta.
- **Ventas**: Escáner con cámara del teléfono/computadora, sonido al escanear, debounce anti-doble lectura, atajos de teclado, carrito, cancelar/devolver ventas.
- **Ganancias**: Cálculo automático de utilidad (precio venta − costo) visible en carrito, ventas y reportes.
- **Alertas**: Aviso de stock bajo.
- **Reportes y Gráficas**:
  - Ventas y ganancias generales (hoy / 7 días / histórico)
  - Productos más vendidos
  - Gráfica individual por producto
- **Exportar** a Excel (CSV)
- **Copia de seguridad** (descargar / restaurar datos)
- **Contraseña** simple de protección
- **Modo oscuro**
- **Diseño moderno y responsive** (funciona en celular y computadora)
- **PWA**: Se puede instalar en el teléfono como aplicación (incluye Service Worker)

## Cómo usar (rápido)

1. Abre el archivo `index.html` en Chrome o Edge (recomendado).
2. La contraseña inicial es: `1234` (cámbiala en Configuración).
3. Agrega productos (puedes poner descripción detallada: "Anillos de plata 925", "Pelotas de basket n.º 7", etc.).
4. Genera códigos de barras, imprímelos y pégalos en tus productos.
5. En la pestaña **Vender** usa la cámara para escanear. Cada venta se guarda y se calcula la ganancia automáticamente.

## Antes de subir

Descarga los 3 archivos indicados en `lib/LEEME.txt` y ponlos dentro de la carpeta `lib/` (para que funcione sin internet).

## Subir a GitHub + GitHub Pages

1. Crea un repositorio nuevo en GitHub.
2. Sube todos los archivos de esta carpeta (`index.html`, `manifest.json`, `sw.js`, `README.md`).
3. Ve a **Settings → Pages**.
4. Source: Deploy from a branch → `main` → `/ (root)`.
5. Guarda. En unos minutos tendrás una URL tipo: `https://tuusuario.github.io/nombre-repo`

## Convertir en APK (Android)

1. Publica la app en GitHub Pages.
2. Entra a [https://www.pwabuilder.com](https://www.pwabuilder.com)
3. Pega la URL de tu GitHub Pages.
4. Sigue los pasos y descarga el APK.
5. El APK pedirá los permisos de **cámara** y almacenamiento automáticamente.

## Permisos

- Cámara (para escanear códigos de barras)
- Almacenamiento (para descargar códigos, backups y CSV)

## Notas importantes

- Los datos se guardan en el navegador (localStorage). Haz copias de seguridad frecuentes.
- Funciona mejor en **Chrome** (Android y PC) y **Safari** (iPhone).
- La primera vez que uses la cámara te pedirá permiso.

---

Hecho para tiendas de abarrotes y negocios similares.
