# IA_minibots_T4_Programaci-n_Genetica

## Descripción

En este documento se presentan los ejercicios desarrollados correspondientes a la sección **4.12 – Ejercicios**, enfocados en el uso de **Programación Genética (PG)** para la solución de problemas de control y optimización.

Se seleccionaron los ejercicios **3 y 4**, los cuales abordan la generación de comportamientos mediante evolución automática de programas.

---

## Ejercicio 3 — Robot repartidor de galletas

### Planteamiento del problema

Se propone un escenario en el cual un robot debe desplazarse dentro de una sala cuadrada para entregar galletas a un grupo de ingenieros distribuidos en posiciones dentro del espacio.

Cada vez que un ingeniero recibe una galleta, el sistema obtiene una recompensa (puntos). El objetivo de la programación genética es encontrar el recorrido o estrategia de movimiento que maximice la cantidad de entregas realizadas.

---

### Representación del problema

#### Conjunto de terminales

Los terminales representan las entradas disponibles para el programa evolutivo:

* Posición actual del robot (x, y)
* Posiciones de los ingenieros
* Distancia al ingeniero más cercano
* Estado de entrega (ingeniero atendido / no atendido)
* Dirección actual del robot

#### Conjunto de funciones

Las funciones corresponden a las operaciones que el programa puede ejecutar:

* Mover adelante
* Girar izquierda
* Girar derecha
* Avanzar hacia objetivo
* Condicional (if)
* Secuencias de acciones
* Comparaciones de distancia

Estas funciones permiten generar estrategias de navegación dentro del entorno.

---

### Función de aptitud

La función de aptitud se definió como:

* Número total de ingenieros atendidos (entregas realizadas)
* Penalización por movimientos innecesarios
* Penalización por colisiones o salidas del área

El objetivo es maximizar el número de entregas con el menor costo de desplazamiento posible.

---

## Ejercicio 4 — Control mediante Programación Genética

### Análisis del video

El video presenta la aplicación de técnicas evolutivas para generar comportamientos de control de manera automática, mostrando cómo un sistema puede aprender estrategias sin programación explícita, únicamente mediante evaluación de desempeño y evolución.

Este enfoque se basa en la idea de que la programación genética puede descubrir soluciones eficientes incluso cuando no se conoce una estrategia óptima previamente.

---

### Ejemplo propuesto de control

Se desarrolló un ejemplo de control en el cual un agente debe mantener una variable dentro de un rango objetivo (por ejemplo, posición o velocidad).

El sistema evoluciona expresiones matemáticas que determinan la acción de control en función del error entre el valor actual y el valor deseado.

---

### Conjunto de terminales

* Error actual
* Error previo
* Valor objetivo
* Variable de estado

---

### Conjunto de funciones

* Suma
* Resta
* Multiplicación
* División protegida
* Funciones condicionales
* Constantes aleatorias

---

### Función de aptitud

La función de aptitud evalúa:

* Error acumulado respecto al valor objetivo
* Estabilidad del sistema
* Penalización por oscilaciones excesivas

El objetivo es minimizar el error total del sistema durante la simulación.

---

## Tecnologías utilizadas

* Python
* Librerías de computación evolutiva (por ejemplo DEAP u otras)
* Simulación numérica
* Procesamiento paralelo (cuando aplica)

---

## Conclusiones

La programación genética permite generar soluciones de forma automática mediante procesos evolutivos, siendo especialmente útil en problemas donde la estrategia óptima no es evidente o es difícil de modelar matemáticamente.

Los ejercicios desarrollados demuestran que es posible:

* Evolucionar comportamientos de navegación
* Generar leyes de control automáticamente
* Optimizar estrategias mediante selección y mutación

---

## Autor

Nombre: _______________________
Curso: ________________________
Fecha: ________________________
