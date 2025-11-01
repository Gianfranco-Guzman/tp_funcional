# TP Programación Funcional – Java (Streams)

Resolución de los ejercicios propuestos aplicando **Streams**, **Lambdas** y **Collectors** en Java.

## Requisitos
- **Java 17** o superior
- **Gradle** (solo si querés correr desde consola; desde el IDE alcanza)

## Estructura del proyecto
src/main/java/org/utn/tpfuncional/
├─ Ejercicio1.java # Alumno(nombre, nota, curso)
├─ Ejercicio2.java # Producto(nombre, categoria, precio, stock)
├─ Ejercicio3.java # Libro(titulo, autor, paginas, precio)
└─ Ejercicio4.java # Empleado(nombre, departamento, salario, edad)


Cada clase tiene su **propio `main()`** para ejecutar y probar de forma independiente.

## Cómo ejecutar
1. Abrí el proyecto en IntelliJ o VS Code.
2. Navegá a `src/main/java/org/utn/tpfuncional/`.
3. Abrí la clase del ejercicio que quieras probar (`Ejercicio1`, `Ejercicio2`, etc.).
4. Presioná **Run** (la flecha verde del IDE).

## Descripción de los ejercicios

### Ejercicio 1 — Alumno(nombre, nota, curso)
- Aprobados (nota ≥ 7) en **MAYÚSCULAS** y **ordenados**.
- **Promedio** general de notas.
- **Agrupar** alumnos por curso (`Collectors.groupingBy`).
- **Top-3** mejores notas.

### Ejercicio 2 — Producto(nombre, categoria, precio, stock)
- Productos con **precio > 100** ordenados **descendente** por precio.
- **Stock total por categoría** (`groupingBy` + `summingInt`).
- **String** con `nombre - $precio` **separado por `;`** (`joining`).
- **Promedio** de precios **general** y **por categoría**.

### Ejercicio 3 — Libro(titulo, autor, paginas, precio)
- **Títulos** con **más de 300 páginas**, **ordenados** alfabéticamente.
- **Promedio de páginas**.
- **Libros por autor** (`groupingBy` + `counting`).
- **Libro más caro** (`max` + `comparing`).

### Ejercicio 4 — Empleado(nombre, departamento, salario, edad)
- Empleados con **salario > 2000**, **ordenados** por salario **descendente**.
- **Salario promedio** general.
- **Suma de salarios por departamento** (`groupingBy` + `summingDouble`).
- **2 empleados más jóvenes** (`sorted` + `limit`).

## Notas
- Paquete de todas las clases: `org.utn.tpfuncional`.
- Cada clase imprime por consola los resultados solicitados.
- Archivos de IDE y compilación están ignorados en `.gitignore`.

## Ejecución rápida
- **Ejercicio 1:** abrir `Ejercicio1.java` → Run
- **Ejercicio 2:** abrir `Ejercicio2.java` → Run
- **Ejercicio 3:** abrir `Ejercicio3.java` → Run
- **Ejercicio 4:** abrir `Ejercicio4.java` → Run  
