# Catálogo 3D

Tienes dos páginas:

- **`index.html`** → la que ven tus clientes. Tiene buscador con lupa, cantidad por producto, carrito y botón para enviarte el pedido por WhatsApp.
- **`admin.html`** → tu panel. Ahí agregas foto, nombre y precio, configuras tu WhatsApp y presionas **Publicar**.

El catálogo vive en `catalogo.json`. El panel lo actualiza solo; no necesitas editar código.

## 1. Subirlo a GitHub (una sola vez)

1. Crea un repositorio nuevo en [github.com](https://github.com) (por ejemplo `catalogo-3d`, público).
2. **Add file → Upload files** y sube estos 5 archivos: `index.html`, `admin.html`, `style.css`, `catalogo.json`, `README.md`. Luego **Commit changes**.
3. Ve a **Settings → Pages**. En *Branch* elige `main` y carpeta `/ (root)`, y presiona **Save**.
4. En 1–2 minutos tendrás tus dos links:
   - Clientes: `https://TU-USUARIO.github.io/catalogo-3d/`
   - Tu panel: `https://TU-USUARIO.github.io/catalogo-3d/admin.html`

Solo compartes con tus clientes el primero.

## 2. Crear tu token de GitHub (una sola vez)

El token es la llave que permite al panel guardar cambios en tu repositorio. Sin él, nadie puede modificar tu catálogo, aunque encuentren `admin.html`.

1. En GitHub: tu foto → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. Ponle un nombre (ej. `panel catalogo`) y una fecha de vencimiento.
3. En **Repository access** elige **Only select repositories** y marca tu repositorio.
4. En **Permissions → Repository permissions** busca **Contents** y ponlo en **Read and write**.
5. **Generate token** y copia el texto que empieza con `github_pat_…`. Solo se muestra una vez.

Trátalo como una contraseña: no lo compartas.

## 3. Usar el panel

1. Abre `admin.html`.
2. **Tu negocio**: escribe el nombre y **tu WhatsApp con código de país** (Perú: `51987654321`). Ahí te llegarán los pedidos.
3. **Productos**:
   - **＋ Nuevo producto**: toca el recuadro para poner la foto, escribe el nombre y el precio.
   - **Subir varias fotos**: eliges muchas fotos de una vez y se crea un producto por cada una. Solo completas nombre y precio.
4. **Publicar**: en *Conexión con GitHub* pega tu usuario, el nombre del repositorio y el token. Presiona **Publicar cambios**.
5. En 1–2 minutos los cambios aparecen en el link de tus clientes.

La barra de abajo te avisa si hay **cambios sin publicar**. Tus ediciones se guardan como borrador en ese navegador, así que puedes cerrar y seguir después.

**Alternativa sin token:** botón **Descargar catalogo.json** y súbelo a GitHub reemplazando el que ya está.

## 4. Cómo lo usa tu cliente

1. Entra al link y escribe en la lupa para encontrar productos.
2. Elige la cantidad con **−** y **+** (o escribiéndola) y presiona **Agregar**.
3. Abre **Mi pedido**, revisa cantidades y total, y presiona **Enviar pedido por WhatsApp**.
4. Te llega a tu WhatsApp un mensaje así, y tú le confirmas:

```
Hola, quiero hacer este pedido en Mi Taller 3D:

• 2 x Pikachu — S/ 30
• 1 x Dragón articulado — S/ 25

Total: S/ 55
```

## Consejos

- **¿Producto con y sin llavero?** Crea dos productos: «Pikachu» y «Pikachu con llavero», cada uno con su precio.
- **Fotos:** el panel las reduce automáticamente para que el catálogo cargue rápido. Con 60–80 productos conviene no pasarse de eso.
- **Más privacidad:** si quieres que nadie adivine la dirección de tu panel, renombra `admin.html` a algo como `panel-taller-x7.html`.
- **Los cambios no se ven:** espera 2 minutos y recarga. Si usas el celular, cierra y abre el navegador.
