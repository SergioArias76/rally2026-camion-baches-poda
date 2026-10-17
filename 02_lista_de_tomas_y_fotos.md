# Lista de tomas, fotos y modelos 3D

Guarden todo en las carpetas de al lado: `clips/` para los videos, `fotos/` para las fotos y `modelos_3d/` para los escaneos 3D.
Nombren los archivos con el bloque del guion, por ejemplo `02_bache_auto.mp4` o `03_cajon_celulares.jpg`.

## 1. Tomas en la calle (Trelew)

| # | Toma | Cómo | Para la escena |
|---|---|---|---|
| 1 | Camión recolector pasando | De lejos, sin patentes ni caras. Si pueden, una toma de varios segundos mientras dobla una esquina. | El gancho / Cierre |
| 2 | Bache visto desde un auto | Celular a la altura del parabrisas, mirando adelante y abajo, como lo vería el celular de adelante. Plano fijo de 5 s. | El problema |
| 3 | Montón de poda en la vereda | Desde la ventanilla del acompañante, a 3 o 4 m, como lo vería el celular derecho. Hagan 2 o 3 lugares. Si pueden, uno de la vereda de enfrente desde la ventanilla del chofer, a ~8 m. | El problema |
| 4 | Vecino junto a su montón (opcional) | Solo con permiso firmado. Plano medio, sin hablar a cámara. | El problema |

**Consejos:** filmen a la mañana o a la tarde, cuando la luz es más linda. Celular horizontal y estable (apoyado o con las dos manos). Mínimo 1080p.

## 2. La prueba con el auto (viernes al mediodía)

Es lo más valioso del video: muestra que el sistema funciona entero, con datos medidos. Necesitan **los tres celulares** y una salida de ~10 km.

| # | Toma | Cómo |
|---|---|---|
| 5 | Montaje | Un celular arriba al centro del parabrisas (mirando la calle), otro en el vidrio del acompañante (vereda derecha) y otro arriba en el vidrio del chofer (vereda de enfrente), sin tapar el espejo. Filmen cómo los ponen. |
| 6 | Vista desde el asiento de atrás | Se ven los tres celulares sacando fotos y la calle de fondo. 10 s mientras manejan despacio. |
| 7 | Pantalla de la app | Grabación de pantalla de cada celular con el contador de fotos subiendo. |
| 8 | Fotos de ejemplo | Elijan 2 fotos seguidas de un mismo bache y 2 de un mismo montón: muestran que cada objeto sale en dos fotos. |
| 9 | La subida | Los celulares conectándose al Wi-Fi y las fotos llegando a la computadora o al servidor. |

**Anoten para el video:** kilómetros recorridos `[X]` y fotos sacadas `[Y]`.

## 3. En la mesa (viernes a la mañana)

| # | Toma | Cómo |
|---|---|---|
| 10 | Cajón con celulares viejos | Una mano saca tres. |
| 11 | El celular arranca solo | El celular sin batería, enchufado a la fuente: se prende solo y abre la app. Es la prueba de que funciona sin batería. Filmen de corrido, sin cortes. |
| 12 | Regulador y kit de dashcam | Si los consiguieron, las piezas solas y después conectadas. |

## 4. La IA y el mapa (viernes a la noche y sábado)

| # | Toma | Cómo |
|---|---|---|
| 13 | Etiquetado | Grabación de pantalla de Roboflow o CVAT dibujando cajas sobre baches y montones de poda. |
| 14 | Entrenamiento | La curva de entrenamiento de RF-DETR en Colab. |
| 15 | Detecciones reales | Fotos de la prueba con los recuadros que puso el modelo, aciertos y errores. |
| 16 | El mapa real | El mapa con los puntos de la salida en auto. |
| 17 | El conteo a mano | La planilla de las 10 cuadras contadas a mano, al lado de lo que encontró el modelo. Sale la precisión `[Z]`. |

> El conteo a mano tiene que ser en un **barrio que no se usó para entrenar**. Si no, el modelo "se acuerda" de las mismas cuadras y el número miente.

## 5. Fotos de los materiales del kit

Fondo liso (una cartulina blanca o gris), luz de ventana de costado y el objeto apoyado o en un trípode.

| Material | Fotos |
|---|---|
| Celulares en desuso | Frente, dorso (que se vea la cámara) y el hueco de la batería vacío. |
| Soportes con sopapa | Solos, y con el celular puesto. |
| Regulador 12/24 V → 4 V | Solo, y conectado al celular. |
| Kit de cableado de dashcam | Solo, con el temporizador a la vista. |
| Servidor (mini PC o Raspberry Pi) | Solo, y con el disco conectado. |
| Kit completo | Todas las piezas separadas sobre la mesa ("flat lay", desde arriba) y después armado. |

**Video giratorio (efecto 3D sin programas):** pongan el kit sobre un plato giratorio o un banquito que gire y filmen 10 segundos mientras da una vuelta. Queda muy bien en la escena de "La idea".

## 6. Modelos 3D reales (opcional, se ve muy bien)

Pueden escanear en 3D los materiales o un montón de poda con el celular y verlos en el visor:

1. Instalen **Scaniverse** o **Polycam**. Tienen versión gratuita y funcionan en muchos celulares con la cámara (fotogrametría). En iPhone Pro usan LiDAR.
2. Caminen alrededor del objeto despacio, con buena luz, a unos 50 cm del objeto (o 1–2 m si es un montón de poda).
3. Exporten el modelo como **.glb** y guárdenlo en `modelos_3d/`.
4. En el visor 3D, vayan al modo **2 · Kit → Cargar modelo 3D (.glb)**. El modelo aparece al lado del kit y se puede girar.

> Revisen antes cuánto permite exportar la versión gratuita de cada app, porque cambia seguido.

## 7. Capturas de pantalla para el reporte y el video

Ya están en `fotos/capturas_visor_3d/`. Si quieren otras:

- Recorrido con las tres ventanas de las cámaras.
- Cámara adelante con la zona útil y la vista previa de la IA.
- El panel **Servidor de la base** con las fotos analizadas.
- Vista aérea con los baches y montones por color.
- Kit despiezado y armado.

Para sacarlas usen **Cmd+Shift+4** en Mac o **Win+Shift+S** en Windows.
