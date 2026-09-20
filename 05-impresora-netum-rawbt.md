# Configurar la impresora NETUM NT-1809 con RawBT

Este manual explica cómo dejar lista la impresora térmica NETUM NT-1809 para que TaxiGP imprima los tickets automáticamente al finalizar cada carrera. TaxiGP no imprime directamente: le manda el ticket a una app llamada **RawBT**, y es RawBT quien habla con la impresora por Bluetooth.

## Lo que hace falta

- La impresora térmica NETUM NT-1809 cargada (o enchufada) y encendida.
- Un móvil Android con Bluetooth.
- La app **RawBT Print Service** (gratuita, se instala desde Google Play). Si no la tienes, la propia app TaxiGP te avisa y te lleva directamente a instalarla la primera vez que intentas imprimir un ticket.

## Paso 1: Emparejar la impresora por Bluetooth

1. Enciende la impresora NETUM (botón de encendido, suele tener un piloto que se pone en verde o azul).
2. En el móvil, ve a **Ajustes → Conexiones → Bluetooth** y actívalo.
3. Dale a **Vincular nuevo dispositivo** / **Buscar dispositivos**.
4. Te debería aparecer algo como "NT-1809", "Printer" o un nombre parecido con "NETUM". Selecciónala.
5. Si pide un código (PIN) para emparejar, prueba con **0000** o **1234** (son los códigos habituales de estas impresoras térmicas).
6. Cuando aparezca como "Conectado" o "Emparejado" en la lista de Bluetooth del móvil, este paso está hecho.

## Paso 2: Instalar RawBT

1. Abre Google Play Store en el móvil.
2. Busca **RawBT Print Service** (el icono es una impresora sobre fondo naranja/rojo).
3. Instálala.

(Si ya intentaste imprimir un ticket desde TaxiGP y no tenías RawBT, la propia app te habrá enseñado un aviso con un botón "INSTALAR RAWBT" que te lleva directo a esta misma app en la Play Store.)

## Paso 3: Configurar RawBT para que use la NETUM

1. Abre la app **RawBT** (no hace falta crear cuenta ni nada, es solo un puente).
2. Busca el apartado de **conexión de la impresora** (suele estar en el menú principal o en un icono de engranaje/ajustes).
3. Elige **Bluetooth** como tipo de conexión.
4. En la lista de dispositivos Bluetooth, selecciona la impresora NETUM que ya emparejaste en el Paso 1.
5. En el tamaño de papel, elige **58 mm** (es el ancho de rollo que usa la NT-1809).
6. Si RawBT ofrece una opción de "imprimir ticket de prueba", pruébala: debería salir un texto de ejemplo por la impresora. Si sale, ya está todo conectado correctamente.

## Paso 4: Usar TaxiGP con la impresora ya lista

Con estos pasos hechos una vez, ya no hay que volver a tocar nada: cada vez que finalizas una carrera en TaxiGP y le das a **"FINALIZAR E IMPRIMIR"**, la app manda el ticket a RawBT automáticamente y este lo imprime solo en la NETUM. También puedes reimprimir cualquier ticket antiguo desde el **Historial de carreras** de TaxiGP, con el botón "REIMPRIMIR".

## Si algo no funciona

- **No imprime nada:** revisa que el Bluetooth del móvil esté encendido y que la impresora siga emparejada (a veces el móvil "olvida" el emparejamiento si pasa mucho tiempo sin usarla — repite el Paso 1).
- **La impresora está encendida pero no aparece en la lista de Bluetooth:** apágala y enciéndela de nuevo, y espera unos 10 segundos antes de buscarla otra vez.
- **Imprime símbolos raros o corta el papel mal:** entra en RawBT y revisa que el tamaño de papel esté en 58 mm, no en 80 mm.
- **Se queda sin papel a mitad de ticket:** cambia el rollo de papel térmico (el lado brillante/sensible va hacia el cabezal de impresión, no hacia fuera).
- **La batería de la impresora se agota rápido:** cárgala completa antes de cada turno; las impresoras térmicas Bluetooth gastan bastante batería si se imprime mucho.
