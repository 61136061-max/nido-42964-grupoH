# Registro de Uso de Inteligencia Artificial — Nido (`nido-huallata`)

- **NRC:** 42964 (lunes)
- **Grupo / Ficha:** Grupo E (`nido-huallata`)
- **Integrantes:**
  - Jefferson Fabricio Suena Mamani (`61136061-max`)
  - David Junior Sotomayor Huayhuacuri (`73440362-sys`)
  - Yael Sebastian Luque Negreros (`yael-luque`)
  - Cristopher Emanuel Lopez Bravo (`cristopher-lopez`)

---

## Declaración de uso

De acuerdo con las normas de probidad académica de la asignatura, el equipo utilizó **Gemini** únicamente como herramienta de **apoyo conceptual** para comprender el funcionamiento de las estructuras de datos (ABB, matriz de adyacencia y DFS recursivo) y resolver dudas sobre mensajes de compilación en C++. En ningún caso se utilizó IA para escribir, completar o reescribir el código fuente ni los entregables del proyecto.

---

## Registro de consultas

| # | Integrante | Herramienta | Qué preguntamos | Qué aprendimos | Cómo lo comprobamos |
| :-: | :--- | :---: | :--- | :--- | :--- |
| 1 | Jefferson Suaña | Gemini | ¿Cómo funciona el paso por referencia de punteros (`Nodo*& r`) al insertar y liberar nodos en un Árbol Binario de Búsqueda en C++? | Comprendimos por qué `Nodo*&` permite modificar directamente los enlaces `izq` y `der` del nodo padre sin perder la referencia al retornar de la recursión, y cómo aplicar el recorrido en postorden para liberar memoria con `delete`. | Implementando un ejemplo pequeño de ABB en Dev-C++ con 5 números enteros y verificando que todos los nodos se enlazaran y liberaran correctamente. |
| 2 | David Sotomayor | Gemini | En un grafo dirigido representado con matriz de adyacencia `M[u][v]`, ¿cómo se diferencia el grado de entrada del grado de salida? | Aprendimos que si la fila `u` representa a quiénes sigue `u` (`M[u][v] = 1`), entonces recorrer la fila `u` calcula el grado de salida (seguidos), mientras que recorrer la columna `u` (`M[x][u] = 1`) obtiene el grado de entrada (seguidores). | Trazando a mano una matriz dirigida de 4×4 en papel antes de escribir las funciones de recorridos por fila y columna. |
| 3 | Yael Luque | Gemini | ¿Por qué guardar un ABB en preorden permite reconstruir exactamente la misma estructura al volver a insertarlo, a diferencia de guardarlo en enorden? | Entendimos que en preorden cada nodo padre se guarda antes que sus hijos izquierdo y derecho, garantizando las mismas comparaciones al reinsertar; mientras que en enorden los elementos salen ordenados y generan un árbol degenerado (lista enlazada). | Dibujando ambos árboles de reconstrucción con ejemplos de palabras y validando que la altura y los recorridos coincidieran tras recargar el archivo. |
| 4 | Cristopher Lopez | Gemini | ¿Cómo evitar ciclos infinitos en un recorrido DFS recursivo sobre un grafo dirigido y qué significa el warning `comparison of integer expressions of different signedness` en C++11? | Comprendimos el uso de un arreglo booleano `visto[]` marcado antes de explorar los vecinos para evitar bucles en ciclos dirigidos, y cómo corregir comparaciones entre `int` y `size_t` (`.length()`). | Probando un grafo dirigido con ciclos de 3 vértices en consola y compilando en Dev-C++ sin advertencias. |
