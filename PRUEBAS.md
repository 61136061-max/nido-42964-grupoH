# Pruebas

| ID | Requisito | Orden o secuencia | Resultado esperado | Resultado obtenido | OK |
|---|---|---|---|---|---|
| P01 | R1 | `registrar @kiwi` (dos veces) | La segunda vez: `E: No se pudo registrar @kiwi` |`E: No se pudo registrar @kiwi`  | ok |
| P02 | R1 | `registrar kiwi` (sin @) | `E: No se pudo registrar kiwi` | `E: No se pudo registrar kiwi` | OK |
| P03 | R2 | `arbol` y `usuarios` |`Preorden: @mango @byte @andes @cuy @lofi @kiwi @pixel @nova @zenit` / `Nodos: 9 \| altura: 5 \| hojas: 4` / `Usuarios (enorden): @andes @byte @cuy @kiwi @lofi @mango @nova @pixel @zenit` | `Preorden: @mango @byte @andes @cuy @lofi @kiwi @pixel @nova @zenit` / `Nodos: 9 \| altura: 5 \| hojas: 4`  |OK| OK |
| P04 | R3 | `seguir @a @a` | `E: Una cuenta no puede seguirse a si misma` | `E: Una cuenta no puede seguirse a si misma` |OK |
| P05 | R4 | `mutuos @zenit` y `popular` |`Mutuos de @zenit (1): @lofi` / `Popular: @mango \| seguidores: 2` | `Mutuos de @zenit (1): @lofi` / `Popular: @mango \| seguidores: 2`  | OK |OK  |
| P06 | R5 | `alcance @mango` y `llega @mango @lofi` |`Alcance de @mango: @byte @cuy @andes @pixel @nova @zenit @lofi \| alcanzados: 7` / `Un post de @mango llega a @lofi: si` | `Alcance de @mango: @byte @cuy @andes @pixel @nova @zenit @lofi \| alcanzados: 7` / `Un post de @mango llega a @lofi: si`  | OK | OK |
| P07 | R6 | `guardar`, `salir`, abrir, `cargar`, `arbol` | El mismo preorden, la misma altura y los mismos seguimientos | `Guardado: 9 cuentas y 9 seguimientos en nido.txt` / `Cargado: 9 cuentas y 9 seguimientos \| altura 5` |OK  |
| P08 | R7 | `hola`, `seguir`, `perfil @nadie` | Mensajes de error; el programa sigue |`hola: orden no encontrada (escribe ayuda)`, `E: No existe `, `E: No existe @nadie`  |OK|

Agreguen todas las que necesiten. Incluyan casos con datos invalidos.
