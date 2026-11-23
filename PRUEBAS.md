# Pruebas

| ID | Requisito | Orden o secuencia | Resultado esperado | Resultado obtenido | OK |
| :-: | :-: | :--- | :--- | :--- | :-: |
| P01 | R1 | `registrar @kiwi` (dos veces) | La segunda vez: `E: No se pudo registrar @kiwi` | `E: No se pudo registrar @kiwi` | OK |
| P02 | R1 | `registrar kiwi` (sin `@`) | `E: No se pudo registrar kiwi` | `E: No se pudo registrar kiwi` | OK |
| P03 | R2 | `arbol` y `usuarios` | `Preorden: @koala @beat @cactus @chasqui @delta @misti @meme @turbo @pixel @zenit` / `Nodos: 10 \| altura: 5 \| hojas: 4` / `Usuarios: @beat @cactus @chasqui @delta @koala @meme @misti @pixel @turbo @zenit` | `Preorden: @koala @beat @cactus @chasqui @delta @misti @meme @turbo @pixel @zenit` / `Nodos: 10 \| altura: 5 \| hojas: 4` / `Usuarios: @beat @cactus @chasqui @delta @koala @meme @misti @pixel @turbo @zenit` | OK |
| P04 | R3 | `seguir @a @a` | `E: Una cuenta no puede seguirse a si misma` | `E: Una cuenta no puede seguirse a si misma` | OK |
| P05 | R4 | `mutuos @pixel` y `popular` | `Mutuos de @pixel (1): @turbo` / `Popular: @turbo (5 seguidores)` | `Mutuos de @pixel (1): @turbo` / `Popular: @turbo (5 seguidores)` | OK |
| P06 | R5 | `alcance @zenit` y `llega @zenit @pixel` | `Alcance de @zenit: @chasqui @turbo @cactus @misti @pixel @delta \| alcanzados: 6` / `si` | `Alcance de @zenit: @chasqui @turbo @cactus @misti @pixel @delta \| alcanzados: 6` / `si` | OK |
| P07 | R6 | `guardar`, `salir`, abrir, `cargar`, `arbol` | El mismo preorden, la misma altura y los mismos seguimientos | Mismo preorden, altura `5` y los mismos seguimientos | OK |
| P08 | R7 | `hola`, `seguir`, `perfil @nadie` | Mensajes de error; el programa sigue | Mensajes de error controlados; el programa sigue ejecutándose | OK |

Agreguen todas las que necesiten. Incluyan casos con datos invalidos.
