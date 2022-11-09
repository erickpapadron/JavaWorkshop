# JavaWorkshop
## Curso de java UASLP encora

#### Mirna Botello / Iván Uresti
## Requisitos del taller
- IntelliJ
- JDK 1.8+
- Cuenta de datos
## Java collections framework
- Interfaces
- Implementaciones
- Algoritmos

---

La clase que implementa la interfaz debe implementar tooodo lo que dice la interfaz, no le importa como, simplemente que lo implemente

Colecciones son estructuras de datos que ya están implementadas

## Beneficio
Todos hablamos el mismo idioma, se mantiene por versiones y van haciendo cambios, más imbargo, l abse sigue siendo la misma.


La idea de los algoritmos, es que todos las colecciones utilicen los mismos métodos.

## Interfaces
### Jerarquía 

#### Collection
- Set
  - SortedSet
- List
- Queue
- Dequeue
---
#### Map (Jerarquí diferente pero aún aśi se dice que es una colección)
- SortedMap
---

## ArrayList
- Arreglo redimensionable
- Complejidad al insertar
   - O(1) Amortized (si tengo que hacer más cosas, pero las puedo despreciar)
- Otras aplicaciones
   - O(n)
- Crece automáticamente cuando se llena

# HashSet
- Elementos no duplicados
- Internamente se usa una hash table (Hash map)
- No ordenada de nunguna forma (ordered, sorted)

Internamente utiliza una hash table

Funciones hash, tenemos una tabla, tenemos un valor y una llave única para cada una de eso

Es una estructura que al final de cuentas es un arreglo

| 0 |
| 1 |
| 2 |


## Métodos equals y hashCode que tienen la clase objetos
### Equals
Nos ayuda para saber si dos objetos son iguales.
## hasCode
Obtiene una función hash con los campos que nosotros le demos a ese objeto.

---
Las java collection asegura que las colecciones son intercambiables, son seguras.

## Preguntas de entrevista

- ¿Qué es una interfaz?
- ¿Cuál es la relación entre Equals y hashCode?
   - Si dos objetos son iguales (equals), su hashCode debe ser el mismo, si esta relación no se cumple, el código se puede romper en cualquier momento.
   - Pero si dos objetos tienen el mismo hashCode, no necesariamente son iguales, la función hash puede tener colisiones, donde generamos con diferentes valores las funciones hash y nos da el mismo valor; en teoría no deberían repetirse, pero pues las cosas pasan. (empalme). Ejemplo con GitHub donde los commit colisionaban provocando que varios repos tivieran el mismo ID haciendo que pasen problemas. 
---

# Complejidad del hash
Constante O(1)

### Implementar nuestras propias colecciones
Solamente para aprender, pero pues usar las de java, duh


# Requerimiento 2
- Nececitamos que las placas puedan ser impresas en orden alfabético
- Tenemos que poder buscar la placa también 😞

## Podemos usar
- TreeSet (ir pensando ese coso para la proxima vez, duh)

https://www.bigocheatsheet.com


## 9 de Noviembre 2022
### Ordered
Obtenemos los datos en el orden en el que fueron insertados

### Sorted
Se ordenan de acuerdo a un criterio, cuando los obtengamos los obtenemos de forma ordenada a diferencia del ***Ordered***


# Nuevo requerimiento
- Placas impresas en orden alfábetico
- buscar placas

---
En una tabla hash 
| 0 |
| :--:|
| 1 | 
| 2 |
| 3 |
| 4 |

### Cubetas/buckets

#### Tablas hsah = Tablas de dispersión

### Árbol: Red Black
Tenemos que saber cómo comparar dos objetos en nuestra lista
# Interfaces
## Comparable
que puede ser comparable con alguien más
## Comparator
Alguién quee compara cosas

### Ojo
Interfaz = Contrato
La interfaz por concepto no debería de permitir implementaciones de métodos, desde java 8, los métodos default existen para meter implementaciones por default a las interfaces, es por eso que la interfaz Comparator puede tener métodos como el de ***reversed()***

## Requerimiento
- Relacionar la información del vehículo con su dueño
- Tenemos un conjunto de archivos que contienen la información de las personas, y un archivo que contiene las relaciones.
- Dado un carro obtener el dueño, donde un carro solo puede tener un dueño, pero un dueño puede tener más de 1 carro

Hash set no se puede iterar en él de manera ordenada, se puede hacer de forma ordered (forma en que fueron insertadas) usando el LinkedHashSet.
HashSet  + LinkedList

## Springboot
https://spring.io/projects/spring-boot
