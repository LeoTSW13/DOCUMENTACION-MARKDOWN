# Tecnológico de Software
## Materia: Fundamentos de álgebra
## Alumno: 1A Pablo Leonardo Noh Vidal 
## Actividad \#16 - Matrices 
---
# Actividad: Análisis y Operaciones con Matrices

Este documento detalla la resolución de tres ejercicios enfocados en la identificación, operación y verificación de propiedades de las matrices.

---

## Ejercicio 1: Clasificación de Matrices

Para las siguientes matrices, se debe determinar su tipo (identidad, diagonal, simétrica o triangular superior) y justificar brevemente la clasificación.

### Matriz A

$\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}$

* *Clasificación:* Matriz Identidad
* *Justificación:* Se clasifica como Identidad ya que su diagonal principal se compone únicamente de 1s y el resto de los elementos son 0.

---

### Matriz B

$\begin{pmatrix} 3 & 0 & 0 \\ 0 & -2 & 0 \\ 0 & 0 & 5 \end{pmatrix}$

* *Clasificación:* Matriz Diagonal
* *Justificación:* Es Diagonal, dado que todos los elementos que están fuera de la diagonal principal son nulos (0).

---

### Matriz C

$\begin{pmatrix} 2 & 1 & 4 \\ 1 & 3 & 5 \\ 4 & 5 & 6 \end{pmatrix}$

* *Clasificación:* Matriz Simétrica
* *Justificación:* Es una matriz Simétrica. Cumple con la condición de que es cuadrada y el elemento aᵢⱼ es igual a aⱼᵢ para todos sus índices (ej. a₁₃ = 4 y a₃₁ = 4).

---

### Matriz D

$\begin{pmatrix} 1 & 2 & 3 \\ 0 & 4 & 5 \\ 0 & 0 & 6 \end{pmatrix}$

* *Clasificación:* Matriz Triangular Superior
* *Justificación:* Se trata de una matriz Triangular Superior, ya que todas las entradas (elementos) que están por debajo de la diagonal principal son cero.

---

## Ejercicio 2: Operaciones Fundamentales

Considerando las siguientes matrices:

*Matriz A:*
$\begin{pmatrix} 2 & -1 \\ 3 & 4 \end{pmatrix}$

*Matriz B:*
$\begin{pmatrix} 5 & 2 \\ -1 & 3 \end{pmatrix}$

Se realizarán las operaciones: *A + B, **2A - B, **A × B, **B × A, y **Aᵗ*.

---

### 2.1. Suma (A + B)

*Cálculo (elemento a elemento):*

| (2 + 5) | (-1 + 2) |
|----------|-----------|
| (3 + -1) | (4 + 3) |

*Resultado:*

$\begin{pmatrix} 7 & 1 \\ 2 & 7 \end{pmatrix}$

*Proceso:* El cálculo se hace sumando los elementos que ocupan la misma posición (misma fila y columna) en ambas matrices.

---

### 2.2. Multiplicación Escalar y Resta (2A - B)

*Paso 1 (2A):*
$\begin{pmatrix} 4 & -2 \\ 6 & 8 \end{pmatrix}$

*Paso 2 (2A - B):*

| (4 - 5) | (-2 - 2) |
|----------|-----------|
| (6 - -1) | (8 - 3) |

*Resultado:*

$\begin{pmatrix} -1 & -4 \\ 7 & 5 \end{pmatrix}$

*Proceso:* Primero, se multiplica la Matriz A por el escalar 2. Luego, se resta la Matriz B al resultado, elemento por elemento.

---

### 2.3. Producto (A × B)

*Cálculo (Fila × Columna):*

| (2×5 + -1×-1) | (2×2 + -1×3) |
|----------------|---------------|
| (3×5 + 4×-1)   | (3×2 + 4×3)  |

*Resultado:*

$\begin{pmatrix} 11 & 1 \\ 11 & 18 \end{pmatrix}$

*Proceso:* Se multiplica cada fila de la Matriz A por cada columna de la Matriz B, sumando los productos resultantes de cada posición.

---

### 2.4. Producto (B × A)

*Cálculo (Fila × Columna):*

| (5×2 + 2×3) | (5×-1 + 2×4) |
|--------------|--------------|
| (-1×2 + 3×3) | (-1×-1 + 3×4) |

*Resultado:*

$\begin{pmatrix} 16 & 3 \\ 7 & 13 \end{pmatrix}$

*Proceso:* Se repite el procedimiento anterior, pero multiplicando las filas de B por las columnas de A. El resultado demuestra que la multiplicación de matrices *no es conmutativa* (A × B ≠ B × A).

---

### 2.5. Transpuesta (Aᵗ)

*Definición:* Se intercambian filas por columnas.

*Resultado:*

$\begin{pmatrix} 2 & 3 \\ -1 & 4 \end{pmatrix}$

*Proceso:* Para obtener la transpuesta, las filas de la matriz original (A) se convierten en las columnas de la nueva matriz (Aᵗ).

---

## Ejercicio 3: Propiedad Asociativa de la Multiplicación

Se utilizarán las siguientes matrices:

*Matriz A:*
$\begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix}$

*Matriz B:*
$\begin{pmatrix} 2 & 0 \\ 1 & 3 \end{pmatrix}$

*Matriz C:*
$\begin{pmatrix} 1 & 1 \\ 0 & 2 \end{pmatrix}$

El objetivo es comprobar la propiedad asociativa: *(A × B) × C = A × (B × C)*.

---

### 3.1. Lado Izquierdo: (A × B)

*Cálculo:*

| (1×2 + 2×1) | (1×0 + 2×3) |
|--------------|--------------|
| (3×2 + 4×1)  | (3×0 + 4×3)  |

*Resultado (A × B):*

$\begin{pmatrix} 4 & 6 \\ 10 & 12 \end{pmatrix}$

---

### 3.2. Lado Izquierdo: (A × B) × C

*Cálculo:*

| (4×1 + 6×0) | (4×1 + 6×2) |
|--------------|--------------|
| (10×1 + 12×0) | (10×1 + 12×2) |

*Resultado Final (Izquierdo):*

$\begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix}$

---

### 3.3. Lado Derecho: (B × C)

*Cálculo:*

| (2×1 + 0×0) | (2×1 + 0×2) |
|--------------|--------------|
| (1×1 + 3×0)  | (1×1 + 3×2)  |

*Resultado (B × C):*

$\begin{pmatrix} 2 & 2 \\ 1 & 7 \end{pmatrix}$

---

### 3.4. Lado Derecho: A × (B × C)

*Cálculo:*

| (1×2 + 2×1) | (1×2 + 2×7) |
|--------------|--------------|
| (3×2 + 4×1)  | (3×2 + 4×7)  |

*Resultado Final (Derecho):*

$\begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix}$

---

### 3.5. Conclusión de la Verificación

*(A × B) × C = A × (B × C)*

$\begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix} = \begin{pmatrix} 4 & 16 \\ 10 & 34 \end{pmatrix}$

✅ *Comprobación:* Se confirma la igualdad. Esto demuestra que la *multiplicación de matrices cumple con la propiedad asociativa*.

---
...








---







