# Acuerdos del Equipo — Nido (`nido-huallata`)

- **Curso:** Estructura de Datos (24UC00428) · NRC 42964 (lunes)
- **Grupo / Comunidad:** Grupo E · `nido-huallata`
- **Repositorio:** `https://github.com/61136061-max/nido-42964-grupoE`

---

## 1. Integrantes y reparto de trabajo

| Integrante | Usuario GitHub | Rol | Lo que le toca |
| :--- | :--- | :--- | :--- |
| Jefferson Fabricio Suaña Mamani | `61136061-max` | Líder y Dev (Árbol) | Ordenar el tablero, juntar ramas en `main`, R1, R2 y R5 |
| David Junior Sotomayor Huayhuacuri | `73440362-sys` | Dev (Grafo) | R3, R4, traza de la matriz a mano y revisión |
| Yael Sebastian Luque Negreros | `yael-luque` | Dev (Persistencia) | R6, R7 y redacción del informe |
| Cristopher Emanuel Lopez Bravo | `cristopher-lopez` | QA y Documentación | Pruebas en consola, `PRUEBAS.md`, `IA.md` y diapositivas |

---

## 2. Cómo nos organizamos

- **Por dónde coordinamos:** Por nuestro grupo de WhatsApp para lo rápido y llamadas por Meet cuando toca avanzar juntos o revisar código.
- **Horarios:** Nos conectamos a partir de las 8:00 p. m. para ver avances, probar el código y aprobar los Pull Requests.
- **Uso de GitHub:** Cada uno avanza su parte en su propia rama para no pisarnos el código en `nido.cpp`. Antes de hacer merge a `main`, otro compañero revisa que compile bien.
- **Si hay dudas o desacuerdos:** Primero probamos el código en Dev-C++ comparándolo con la traza en papel de la Ficha E. Si aún hay dos opciones, lo conversamos en llamada y votamos entre los cuatro.
- **Para la sustentación:** Todos repasamos el árbol, la matriz y el DFS para que cualquiera pueda explicar cualquier parte si el profe pregunta.

---

## 3. Actas de reuniones

### Acta 1 — Organización inicial (Jueves 19/11)
- **Estuvimos:** Jefferson, David, Yael y Cristopher.
- **Qué acordamos:**
  1. Como hubo reordenamiento de grupos en el salón, nos quedamos trabajando los cuatro con la **Ficha E (`nido-huallata`)** y nos repartimos los requisitos R1 al R7.
  2. Armamos el repo en GitHub, agregamos al profesor y creamos los Issues en el tablero.
  3. Pegamos los datos de `nido-huallata` en `nido.cpp`, probamos que compile limpio y subimos el tag `v0.1`.

### Acta 2 — Diseño en papel y avance base (Viernes 20/11)
- **Estuvimos:** Jefferson, David, Yael y Cristopher.
- **Qué acordamos:**
  1. Hicimos a mano el dibujo del árbol con las 10 cuentas y la matriz de 10×10, comprobando que la orden 4 (`seguidores @pixel`) salga igual al punto de control.
  2. Subimos y revisamos por Pull Request las funciones de R1, R2 y R3, verificando que las primeras 10 órdenes den lo mismo que nuestra traza.
  3. Avanzamos los capítulos 1 y 2 del informe y dejamos listo el tag `v0.5`.

### Acta 3 — Cierre, pruebas y entrega final (Domingo 22/11)
- **Estuvimos:** Jefferson, David, Yael y Cristopher.
- **Qué acordamos:**
  1. Terminamos R4, el alcance con DFS (R5), guardar/cargar en `nido.txt` (R6) y la liberación de memoria al salir (R7).
  2. Corrimos toda la secuencia oficial de 27 órdenes y probamos errores a propósito para llenar `PRUEBAS.md` e `IA.md`.
  3. Cerramos el informe en PDF, terminamos las diapositivas para la exposición y dejamos el tag `v1.0` junto con el ZIP listo para subir al aula virtual.
