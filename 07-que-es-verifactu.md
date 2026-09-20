# Qué es eso de "NO VERI*FACTU" que sale en el ticket

Al final de cada ticket que imprime TaxiGP, verás un bloque de texto parecido a este:

```
     NO VERI*FACTU
Factura no enviada a la AEAT
en el momento de su emision
Huella: EBCB625D-B519FF13...
Huella anterior: 7E53B4F8-EA3A9765...
```

No es ningún error ni nada que tengas que arreglar. Te explicamos qué significa:

## La "huella"

Desde julio de 2027, la ley obliga a que las facturas de los autónomos lleven una especie de "sello" que demuestre que nadie las ha podido modificar después de emitirlas. Ese sello es la **huella**: un código único que se calcula con los datos de esa factura (número, importe, fecha...) **y además con la huella de la factura anterior**, formando una cadena. Si alguien intentase cambiar una factura antigua, la cadena dejaría de encajar y se notaría.

TaxiGP calcula esta huella automáticamente en cada factura, sin que tengas que hacer nada. Es la parte de "seguridad e integridad" de la ley, y ya está cumplida.

## "Factura no enviada a la AEAT en el momento de su emisión"

Este aviso indica que, de momento, el ticket **no se transmite en directo a Hacienda** en el mismo instante de imprimirlo (eso es una parte del sistema VeriFactu que se está terminando de preparar). No afecta a tus obligaciones actuales como taxista ni cambia nada en cómo trabajas hoy — simplemente es un aviso técnico que aparece mientras esa parte se completa. Tú sigues emitiendo tus facturas con normalidad, con la huella y todo lo demás ya funcionando.

## ¿Tengo que hacer algo con esto?

No. Es información que la propia app gestiona sola. Tu única responsabilidad, como se explica en el primer uso de la app, es guardar bien tus copias de seguridad (correo y Google Drive) — ver [04-copia-de-seguridad.md](04-copia-de-seguridad.md).
