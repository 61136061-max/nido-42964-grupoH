# Uso de inteligencia artificial

Si no usaron IA, escriban: **No usamos IA.**

| Fecha | Integrante | Herramienta | Que preguntamos | Que aprendimos | Como lo comprobamos |
|---|---|---|---|---|---|
| 20/11/2026 | Jefferson Suaña | Gemini | Cómo plantear casos base en funciones recursivas de árboles binarios (contar hojas, calcular altura y liberar nodos en postorden). | A separar los casos base con condicionales simples (`r == nullptr`) y acumular los retornos de los subárboles izquierdo y derecho sin usar librerías externas. | Practicando con un árbol de ejemplo de 4 nodos en papel y compilando con `g++ -std=c++11` para verificar que no queden fugas de memoria. |
| 21/11/2026 | David Sotomayor | Gemini | Cómo funciona el recorrido en profundidad (DFS) recursivo usando un arreglo de visitados sobre una matriz de adyacencia dirigida. | A marcar cada vértice visitado antes de explorar sus vecinos entrantes para evitar ciclos infinitos en grafos dirigidos. | Trazando a mano el recorrido en un grafo pequeño de 4 vértices y verificando los pasos de visita en consola. |
| 21/11/2026 | Yael Luque | Gemini | Cómo estructurar la lectura y escritura secuencial de datos en C++ con `ifstream` y `ofstream` para guardar un árbol en preorden. | Que al guardar los nodos en preorden se conserva exactamente la misma forma del árbol binario al volver a insertarlos al cargar. | Guardando el estado en `nido.txt`, cerrando el programa, volviendo a cargar y comparando el recorrido `arbol`. |
| 22/11/2026 | Cristopher Lopez | Gemini | Cómo organizar casos de prueba límite (entradas vacías, comandos desconocidos o nodos inexistentes) en una tabla de validación. | A verificar que cada validación con `if` simple controle el error y permita que el bucle principal siga pidiendo órdenes. | Ejecutando las pruebas `P01` a `P08` directamente en la consola de Dev-C++ y anotando las salidas reales. |


Recuerden: se permite preguntar conceptos y practicar con ejemplos que NO son de Nido.
No se permite pedir que escriba, complete o reescriba el codigo, el informe o las respuestas,
ni pegar la consigna, la ficha o el kit.
