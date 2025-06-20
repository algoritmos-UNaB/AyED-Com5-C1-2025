# 2do PARCIAL - Algoritmos y Estructuras de Datos  
### Sábado 21 de junio de 2025

---

## Completar los siguientes datos:

- **Nombre y Apellido**:  
- **Email**:  
- **Comisión**:  

---

## Modalidad del examen

- El parcial estará habilitado para su resolución desde el **sábado 21/06 a las 07:00 hs** hasta el **sábado 21/06 a las 19:00 hs**.
- Cada estudiante tiene **1 (un) solo intento** para resolver la actividad.
- El tiempo máximo disponible para completar el examen es de **4 (cuatro) horas** desde el inicio del intento.
- Las resoluciones deben ser escritas en los archivos correspondientes a cada ejercicio:  
  `ejercicio1.py`, `ejercicio2.py`, etc.
- El tiempo se contabiliza desde el momento en que aceptan realizar la actividad en GitHub Classroom.
- Solo se aceptarán **commits realizados dentro de las 4 horas** de iniciado el intento.
- Los resultados serán publicados a más tardar el **lunes 23 de junio luego de las 20:00 hs**.

> ⚠️ **NOTA IMPORTANTE:** DEBEN COMPLETAR LA PARTE SUPERIOR DE ESTE README CON SUS DATOS ANTES DE COMENZAR.

---

# EJERCICIOS

---

### **¡Tributos, Pilas y Colas! Estructuras de Datos en _Los Juegos del Hambre_**

---

### Parte I: Introducción

Bienvenido a tu prueba final para convertirte en un **Vigilante del Capitolio**.  
Tu tarea es supervisar una simulación simplificada de los Juegos del Hambre, utilizando estructuras de datos fundamentales para organizar a los tributos, sus alianzas y los eventos dentro de la Arena.

> El éxito de los Juegos depende de tu capacidad para modelar información de manera eficiente utilizando tus propios algoritmos y estructuras.

---

### Parte II: Ejercicios Prácticos

---

### 🏹 Ejercicio 1: La Cosecha  
**(Archivos y Listas Enlazadas Simples)**

**Narrativa:**  
La Cosecha ha finalizado y recibiste un archivo `tributes.txt` con los tributos seleccionados. Debes organizar la información por distrito.

**Formato del archivo de entrada (`tributes.txt`):**
```
Katniss Everdeen;12;Arquería  
Peeta Mellark;12;Fuerza  
Clove;2;Cuchillos  
Cato;2;Espada  
Rue;11;Agilidad  
Thresh;11;Fuerza  
```

**Tarea:**

- Crear una clase `TributeNode` que almacene `nombre`, `distrito`, `habilidad`, y `next`.
- Implementar la función `procesar_cosecha(ruta_archivo)` que lea el archivo y organice los tributos en una lista de 13 posiciones (índices del 1 al 12), cada una conteniendo la **cabeza de una lista enlazada simple** con los tributos de ese distrito.

---

### 🤝 Ejercicio 2: Alianzas en la Arena  
**(Manipulación de Listas Enlazadas)**

**Narrativa:**  
Durante los Juegos, los tributos pueden formar alianzas temporales que cambian con el tiempo.

**Tarea:**

- Crear una clase `GestorAlianzas` con métodos:
  - `crear_alianza(lista_nodos_tributos)`
  - `eliminar_tributo(nombre_tributo, cabeza_alianza)`

Debe contemplarse correctamente el caso en el que el tributo a eliminar sea el primero de la alianza.

---

### 🚂 Ejercicio 3: El Tren de Suministros del Capitolio  
**(Lista Doblemente Enlazada + Fila)**

**Narrativa:**  
El Capitolio envía un tren con recursos a la Arena. Cada vagón transporta una categoría de suministros, y cada categoría contiene una fila de artículos.

**Tarea:**

1. Implementar una clase `Queue` usando nodos enlazados:
   - Métodos: `enqueue`, `dequeue`, `is_empty`.
2. Crear una clase `WagonNode` para representar un vagón:
   - Contiene `category`, `supply_queue`, `next`, `prev`.
3. Crear la clase `SupplyTrain` para gestionar la lista doblemente enlazada:
   - Métodos:
     - `add_wagon(category)`
     - `load_supply(category, item)`
     - `dispatch_supply(category)`
     - `print_train_forward()`

**Objetivo:**  
Modelar un sistema que combine listas doblemente enlazadas y colas, manipulando punteros en ambas direcciones.

---

### 📺 Ejercicio 4: Eventos del Capitolio y Ordenamiento  
**(Pilas y Algoritmos de Ordenamiento)**

**Narrativa:**  
Los Vigilantes lanzan eventos en la Arena, y el Presidente Snow necesita informes de tributos ordenados por habilidad.

**Tareas:**

1. **Pila de Eventos:**
   - Implementar una clase `PilaEventos` usando una lista de Python.
   - Métodos: `agregar_evento`, `lanzar_evento`, `ver_proximo_evento`.

2. **Ordenamiento:**
   - Implementar la función `ordenar_por_habilidad(lista_tributos)`.
   - Ordenar alfabéticamente por el campo `habilidad` usando **Insertion Sort**, implementado desde cero.

---

### Parte III: Preguntas Teóricas

---

#### 1. Diferencias entre Listas y Listas Enlazadas

- ¿En qué situaciones es preferible usar una lista enlazada en lugar de una lista tradicional?
- ¿Cuál es la principal desventaja de las listas enlazadas respecto al acceso por índice?

---

#### 2. Pilas y Colas

- Explica la diferencia entre una pila (LIFO) y una cola (FIFO) con un ejemplo de la vida real.
- ¿Por qué las pilas son útiles para el manejo de eventos o deshacer acciones?

---

#### 3. Complejidad de Búsqueda

- ¿Cuál es la complejidad de buscar un elemento en una lista desordenada? ¿Y en una lista ordenada?
- ¿Por qué la búsqueda binaria solo puede aplicarse a listas ordenadas?

#### 4. Ordenamientos

- ¿Cómo explica Walter Bel el ordenamiento burbuja mejorado?
- ¿Podriamos utilizar el ordenamiento por inserción para ordenar una lista enlazada? ¿Por qué sí o por qué no?

---

#### 5. Estructuras de Datos y Aplicaciones

- Menciona una situación donde sería ventajoso usar una cola en vez de una pila.
- ¿Qué ventajas ofrece una lista doblemente enlazada sobre una simple?


---
> _"¡Que la suerte esté siempre de su lado!"_
