# Facturas para empresa

A veces un cliente necesita que la factura salga a nombre de su empresa (con el NIF de la empresa), no a su nombre particular. TaxiGP tiene esto previsto, pero hay que hacerlo en el momento correcto.

## Cómo marcarlo

Antes de empezar la carrera (o durante, en la pantalla de detalle), marca la casilla **"Factura empresa"** (arriba del taxímetro) o **"Cliente necesita datos de su empresa"** (en el apartado "FACTURA PARA EMPRESA" de la pantalla de detalle).

Importante: **esta casilla se desmarca sola al empezar cada carrera nueva**. Es a propósito — así no se queda marcada por error de una carrera a la siguiente. Si el cliente pide factura de empresa, márcala de nuevo en la carrera de ese cliente.

## Dos casos posibles

**El cliente sabe el NIF de su empresa en el momento:**
Rellena el NIF de empresa y el nombre de empresa en los campos correspondientes. El ticket saldrá ya con esos datos.

**El cliente NO sabe el NIF en el momento** (es lo más habitual):
Deja esos dos campos en blanco. El ticket imprimirá automáticamente un aviso al cliente pidiéndole que te mande los datos de su empresa por WhatsApp, con tu número de teléfono y el número de factura, para que luego le mandes el ticket corregido. Por eso es importante tener bien puesto tu número en el campo **"Tu WhatsApp"** de ese mismo apartado — así sale correcto en el ticket.

## Ejemplo de cómo queda el ticket en este segundo caso

```
       -----CLIENT-----
Datos de empresa pendientes.
Enviamelos por WhatsApp al
605289646 con el numero de
ticket 17 y te mando
el ticket corregido.
```

Cuando el cliente te mande esos datos por WhatsApp, puedes ir al Historial de carreras, buscar ese número de factura, y reimprimir el ticket ya corregido a mano (ver [06-historial-y-reimpresion.md](06-historial-y-reimpresion.md)).
