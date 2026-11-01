# ¿Quieres salir conmigo? 💖

Página de una sola pantalla, pensada para el celular. Cuando ella toca **¡Sí!**,
te llega una notificación al teléfono y salen corazones en su pantalla.
El botón "Por favor..." cambia de frase cada vez que lo toca, se encoge,
y el "¡Sí!" va creciendo.

## Archivos
- `index.html`: toda la página (diseño, lógica y configuración).
- `README.md`: esta guía.

## 1. Cambia la configuración
Abre `index.html` y busca el bloque `CONFIG`:

| Campo | Para qué sirve |
|---|---|
| `NOMBRE` | Nombre que aparece en el mensaje final. |
| `NTFY_CANAL` | Canal secreto de notificaciones. Cámbialo por uno tuyo, largo y difícil de adivinar. |
| `AVISAR_AL_ABRIR` | `true` para que también te avise cuando ella abra el link. |
| `WHATSAPP` | Tu número con código de país, sin `+` (ej. `593991234567`). Opcional. |
| `IMAGEN` | Nombre de una imagen o GIF que subas junto al `index.html`. Opcional. |

## 2. Activa la notificación en tu teléfono
1. Instala la app **ntfy** (Play Store o App Store).
2. Toca **+** y suscríbete al mismo nombre que pusiste en `NTFY_CANAL`
   (servidor por defecto `ntfy.sh`).
3. Prueba que funciona: abre la página y toca **¡Sí!** (la prueba la haces tú, antes de enviarle el link).

> Cualquiera que conozca el nombre del canal podría leer o enviar mensajes en él.
> Por eso conviene que sea largo y raro.

## 3. Publícala en GitHub (desde el celular)
1. Crea un repositorio nuevo en github.com (público).
2. **Add file → Upload files** y sube `index.html`
   (y tu imagen si pusiste una). Confirma con **Commit changes**.
3. Ve a **Settings → Pages**. En *Build and deployment* elige
   **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
4. En uno o dos minutos aparece el link:
   `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`

Ese link es el que le envías.

## Nota sobre la privacidad
GitHub Pages es público. Si no quieres que otras personas lo encuentren, usa un
nombre de repositorio poco obvio y no lo compartas más que con ella.
