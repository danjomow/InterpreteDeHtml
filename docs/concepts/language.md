# Language

Este documento, tiene como proposito ser un blog de notas, para el dominio de
un lenguaje.

##Principios basicos.

### Estructuras de datos

comprendiendo que un "dato", es un elemento logicamente representable. Un
lenguaje de programación, turing complete, es un lenguaje formal, que mediante
cualquier medio de ejecución, puede represetar la logica matematica.

En la computación, el dato basico es el elemento binario.

y su relacion con el computo es el siguiente.

```text
+=---------------=+=-------------=+
|    "Memoria"    |     Dato      |
|                 |               |
|    0x293dfcd    |       1       |
|  Identificador  |  Información  |
+=---------------=+=-------------=+
```

TODO Elemento en la computación respeta esta estructura. sea explicita o
discreta.

Las estructuras de datos, responden a la forma en la que la Información es
organizada o estructurada

Teniendo encuenta lo anterior, todo lenguaje tiene unas estructuras basicas o
por defecto, de datos.

#### Primitivas

- Variables
- Numeros
    - Enteros
    - Racionales - Punto Flotante
- Caracteres de texto
    - ASCII
    - Unicode
- Cadenas estaticas
    - Arreglos
    - Bufferes de Información

#### Complementarias

- Cadenas dinamicas / Iterables
- HashMaps / diccionarios / Key-Value Objects
- Vectores
- Arboles

> [!Nota]
> A partir de este punto cada lenguaje normalmente presenta sus diferencias,
> tuplas, vectores, arboles, o cualquier organización de Información tratada
> desde la perspectiva de "UN" elemento, "una cosa".

---

### Control de flujo

Cada lenguaje ofrece elementos / herramientas, para controlar el flujo de un
proceso.


#### Expresiones Condicionales

La clasica expresión, "IF", es la puerta de entrada al condicionamiento del
flujo, mediante expresiones logicas o condicionales.

```text
+=------------------------------------------------------=+
|  AND  |  OR  |  NOT  |  Equal  |  Greater | Less than  |
+=------------------------------------------------------=+
|       |      |       |         |          |            |
|  &&   |  ||  |   !   |    ==   |   > >=   |    < <=    |
|       |      |       |         |          |            |
+=------------------------------------------------------=+
```
Algunos lenguajes extienden el comportamiento base.

#### Funciones ciclicas

- For Loop
Es un Ciclo que tiene normalmente, un indice, y un limite condicional,
canonicamente, tambien posee una expresión para cada momento  de las
iteraciones, comunmente estiona el aumento del indice.

for (index = 0; index <= 10; index++) {...}

- While

Es un ciclo, que comunmente se utiliza para aplicar acciones o  navegar algún 
volumen de información, por ejemplo una lista. Su estructura normalmente es
una condicion, comunmente relacionada con el limite de iteraciones del ciclo.

while ( list.next != NULL ) {...}

Tambien tiene el la posibilidad de entrar en un posible ciclo infinito, ya que
solo la condición, es su unico limite, esto es comunmente usado en entornos muy
especificos.

while (true) { if(condition) break; }


#### Reserved Staments / Expresiones Reservadas

Las expresiones reservadas, son palabras que dentro del lenguaje tiene alguna
función. Las parabras relacionadas con el control de flujo, pueden ser.

- continue
- break
- return
- default

---

### Condicionales

una expresión condicional normalmente es usada por funciones logicas, tales
como if, y while, o aquella función que tome en sus parametros, condicionales.

Estas condicionales, tienen como resultado "true" o "false", "1" o "0", que es
basicamente el resultado de la tabla de verdad que expresaria la condicional.


```text
+=-------+-----------+---------=+
| lado A | Expresión |  lado B  |
+=-------+-----------+----------+---------=+
|  true  |     &&    |  false   |  false   |
+=----------------------------------------=+
```

tambien los lenguajes ofrecen las expresiones ternarias.

```C

5 > index ?? ifIsTrue() : ifIsFalse()

```

Asi como la función Switch, que condiciona su funcionamiento apartir de casos.

```js

switch( case ) { optionA: ifIsOptionA(); break; Defatul: defaultCase(); }

```
