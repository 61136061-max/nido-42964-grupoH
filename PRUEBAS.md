# Pruebas

| ID | Requisito | Orden o secuencia | Resultado esperado | Resultado obtenido | OK |
| :-: | :-: | :--- | :--- | :--- | :-: |
| P01 | R1 | `registrar @mango` (dos veces) | La segunda vez: `E: No se pudo registrar @mango` | `E: No se pudo registrar @mango` | OK |
| P02 | R1 | `registrar mango` (sin `@`) | `E: No se pudo registrar mango` | `E: No se pudo registrar mango` | OK |
| P03 | R2 | `arbol` y `usuarios` | `Preorden: @koala @beat @cactus @chasqui @delta @misti @meme @mango @turbo @pixel @zenit` / `Nodos: 11 \| altura: 5 \| hojas: 4` / `Usuarios (enorden): @beat @cactus @chasqui @delta @koala @mango @meme @misti @pixel @turbo @zenit` | `Preorden: @koala @beat @cactus @chasqui @delta @misti @meme @mango @turbo @pixel @zenit` / `Nodos: 11 \| altura: 5 \| hojas: 4` / `Usuarios (enorden): @beat @cactus @chasqui @delta @koala @mango @meme @misti @pixel @turbo @zenit` | OK |
| P04 | R3 | `seguir @koala @koala` | `E: Una cuenta no puede seguirse a si misma` | `E: Una cuenta no puede seguirse a si misma` | OK |
| P05 | R4 | `mutuos @pixel` y `popular` | `Mutuos de @pixel (1): @turbo` / `Popular: @turbo \| seguidores: 5` | `Mutuos de @pixel (1): @turbo` / `Popular: @turbo \| seguidores: 5` | OK |
| P06 | R5 | `alcance @zenit` y `llega @zenit @pixel` | `Alcance de @zenit: @chasqui @turbo @cactus @misti @pixel @delta \| alcanzados: 6` / `Un post de @zenit llega a @pixel: si` | `Alcance de @zenit: @chasqui @turbo @cactus @misti @pixel @delta \| alcanzados: 6` / `Un post de @zenit llega a @pixel: si` | OK |
| P07 | R6 | `guardar`, `salir`, abrir, `cargar`, `arbol` | El mismo preorden, la misma altura y los mismos seguimientos | `Guardado: 11 cuentas y 17 seguimientos en nido.txt` / `Cargado: 11 cuentas y 17 seguimientos \| altura 5` | OK |
| P08 | R7 | `hola`, `seguir`, `perfil @nadie` | Mensajes de error; el programa sigue | `hola: orden no encontrada (escribe ayuda)`, `E: No existe`, `E: No existe @nadie` | OK |
| P09 | R3 | `seguidores @pixel` (punto de control) | `Seguidores de @pixel (3): @chasqui @delta @turbo` | `Seguidores de @pixel (3): @chasqui @delta @turbo` | OK |
| P10 | R3, R5 | `dejar @misti @turbo` y `alcance @zenit` | `@misti dejo de seguir a @turbo` / `Alcance de @zenit: @chasqui @turbo @cactus @pixel @delta \| alcanzados: 5` | `@misti dejo de seguir a @turbo` / `Alcance de @zenit: @chasqui @turbo @cactus @pixel @delta \| alcanzados: 5` | OK |

Agreguen todas las que necesiten. Incluyan casos con datos invalidos.
