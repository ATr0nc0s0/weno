# WENO

**Si es chileno, es weno.**

WENO es un lenguaje de etiquetas en español, libre y gratuito, que genera código ZPL para impresoras Zebra. Las medidas van en milímetros, las órdenes son palabras en español y los errores se explican en español.

```
etiqueta 100x60 densidad 203 po
fuente legible

caja @ 2,2 96x10 relleno
texto "ENVÍO EXPRESS" @ 5,4 tam 6 negrita blanco
texto "Valentina Rojas" @ 6,19 tam 6 negrita
barras "NV-2026-004815" @ 6,37 alto 13
qr "https://weno.dev" @ 74,36 tam 20
```

Pruébalo en **https://weno.dev**: escribe a la izquierda, mira la etiqueta en vivo y copia el ZPL.

## Características

- Órdenes en español: `etiqueta`, `texto`, `caja`, `linea`, `circulo`, `barras`, `qr`, `var`, `fuente`, `copias`.
- Medidas en milímetros, posición con `@ x,y` y `@ centro,y`.
- Variables con `{nombre}`, más `{fecha}` y `{hora}`.
- Códigos Code 128, Code 39, EAN-13 y QR.
- Grabación de etiquetas RFID (EPC y memoria de usuario) con la orden `rfid`.
- 9 fuentes libres que se envían como imagen, y todas las fuentes residentes de Zebra con `fuente zebra/…`.
- Tildes y ñ en UTF-8.
- `po` opcional al final de cualquier línea.

## Archivos

Los programas WENO usan la extensión `.weno`.

## Licencia

MIT. Puedes usarlo, modificarlo y distribuirlo libremente, también con fines comerciales.

## Aviso de marcas

ZPL es una marca registrada de Zebra Technologies Corporation. WENO es un proyecto independiente que genera código ZPL; no está afiliado ni respaldado por Zebra.

Creado por Alejandro Troncoso, Chile.
