# Cómo usar el taxímetro

La pantalla principal de TaxiGP funciona como un taxímetro de verdad: tiene un estado **LIBRE** (naranja) y un estado **OCUPADO** (rojo), y los botones cambian según en cuál estés.

## Estado LIBRE — empezar una carrera

Con el taxi libre, ves 4 botones para elegir cómo empieza la carrera:

- **TARIFA URBANA** — para una carrera normal por Barcelona ciudad. La tarifa se calcula sola según dónde estés (automática).
- **TARIFA INTERURBANA** — para carreras que salen de la ciudad. También automática.
- **T-3 · PRECIO CERRADO** — para carreras que vienen de una plataforma (Uber, Bolt, FreeNow...) con un precio ya acordado. Al pulsarlo te pregunta el nombre de la plataforma, y al finalizar te pedirá el precio acordado con ella.
- **T-4 · AEROPUERT·MOLL** — tarifa fija para trayectos al aeropuerto o al puerto (Moll). El precio se pone automáticamente, sin tener que calcularlo.

Antes de pulsar el botón de tarifa, si el cliente te pide factura para su empresa, marca la casilla **"Factura empresa"** que hay arriba del todo — ver el manual [03-facturas-para-empresa.md](03-facturas-para-empresa.md) para más detalle.

## Estado OCUPADO — durante la carrera

Una vez iniciada la carrera, tienes 3 botones:

- **P · PARADA** — congela el taxímetro (por ejemplo, si el cliente para a hacer un recado). El contador de distancia GPS se detiene hasta que vuelvas a moverte.
- **SUPLEMENTOS** — para añadir suplementos (maletas, festivos, nocturnidad, aeropuerto, lo que corresponda). Te deja escribir un importe manual también, por si hay algo que no está en la lista. Hay un botón "PROPONER SEGÚN RECORRIDO" que te sugiere suplementos automáticamente según lo que lleva recorrido la carrera — siempre puedes cambiarlo a mano.
- **L · LIBRE** — finaliza la carrera e imprime el ticket. Es el mismo resultado que darle a "FINALIZAR E IMPRIMIR" en la pantalla de detalle.

## Otros botones (siempre visibles)

- **T/O** — abre la pantalla de Turno: te enseña la fecha/hora y el total cobrado en el día.
- **IR A...** — escribe una calle y número y te abre el navegador (Google Maps u otro) para llevarte hasta ahí.
- **HISTORIAL** — ver todas las carreras guardadas y reimprimir cualquiera (ver [06-historial-y-reimpresion.md](06-historial-y-reimpresion.md)).
- **⚙ (engranaje)** — abre los Ajustes: correo, Google Drive, datos que se muestran en el ticket, etc.

## El botón "+" al sumar suplementos

Cuando estás parado con suplementos añadidos, aparece un botón grande "+" que te deja sumar el total de suplementos al importe que se ve en pantalla, para que tengas de un vistazo el total que vas a cobrar antes de imprimir.

## Precio acordado

Si has quedado con el cliente en un precio cerrado (sin usar taxímetro), marca la casilla **"Precio acordado"** en la pantalla de detalle antes de finalizar: el ticket lo indicará como tal.

## Al finalizar

Cuando finalizas (con "L · LIBRE" o "FINALIZAR E IMPRIMIR"), la app hace todo esto sola, sin que tengas que tocar nada más:

1. Genera el ticket con todos los datos.
2. Lo manda a imprimir a la impresora térmica (a través de RawBT).
3. Lo guarda en el Historial de carreras.
4. Si tienes activado el envío automático por email, lo envía.
5. Si tienes Google Drive conectado, sube una copia a tu carpeta "TaxiGP Facturas".

Todo esto pasa en segundo plano — tú solo tienes que esperar a que salga el papel.
