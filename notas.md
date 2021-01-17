# Introducción al Pensamiento Computacional con Python 

## Modulo I Introduccion al pensamiento computacional

### 01 Introduccion al pensamiento computacional

Breve introduccion de david aroestti sobre para que sirve programar y los usos que el le da a python en su vida diaria laboral

### 02 Introduccion al computo

* El telar de jackart incorporo el computo con punch-cards.

* Motor Analitico de babage, crea una maquina general que podia manejar calculos usando engranes.

* Un problema que resolvio las computadoras fue el censo de estados unidos.

* A final de los 30 Alan Turing y Alonso Church vienen con la maquina imaginaria de la cinta infinita, todos los algoritomos que tenemos como humanidad era la misma secuencia de instrucciones se puede computar matematicamente.

* ENIAC se construye para programarse con cables

* Von Neuman genera la primer computadora donde puedes insertar un programa

* Richard Fayman nos da las bases matematicas para el computo cuantico.

#### Computo y Computadoras

* Las computadoras hacen dos cosas: hacen calculos y recuerdan el resultado de dichos calculos

* Aun con las computadoras modernas existen problemas que no podemos resolver.

### 03 Introduccion a los lenguajes de programacion

#### Conocimiento declarativo vs imperativo

**Declarativo:** nos dice que tipo de relaciones existe entre ciertas variables, entre diersos objetos.

**Impertativo:** nos dice como lograr un objetivo

**Algoritmo:** "Un algoritmo es una lista finita de instrucciones que describen un computo, que cuando se ejecuta con ciertas entradas (inputs) ejectuta pasos intermedios para llegar a un resultado (output)" *John V. Guttag*

Los lenguajes de programacion nacen con ada lovelace, mientras los de alto nivel llegan con Grace Hopper.

##### Programacion

* **Turing completeness**: implementan todos los primitivos que en principio necesitamos para hacer cualquier tipo de algoritmo.

* Los lenguajes de programacion modernos dan primitivos que son mas convenientes que los primitivos de Turing.

##### Lenguajes( Son precisos, exactos, y tienen un solo significado, no son ambuguos)

* **Sintaxis:** Defne al secuencia de simbolos que esta bien formada.

* **Semantica estatica:** Define que eninciados con sintaxis correcta tienen significado.

* **Semantica:** Define el significado. En los lenguajes de programacion solo hay un significado.

## Modulo II Introducción a Python

### 04 Preparacion de tu computadora

Realizamos la configuracion basica para integrar python a tu sistema operativo e instalamos VSCode.

### 05 Elementos Basicos de Python

#### Lenguajes de programacion
No vamos a Aprender python sino que se hablará de los elementos básicos de programación

**Alto nivel:** está diseñado para los humanos. *Pyrthon
**Bajo nivel:** Está optimizado para las computadoras, se acerca mas a los 1/0
**General:**  Que tiene todos los primitivos que nos otorga Turing para poder implementar algoritmos. 
**Dominio Específico:** Están dirigidos hacia aplicaciones muy específicas
**Interpretados:** Mientras correo el programa , después de cada instrucción esta es leída por el programa.
**Compilado:** Se convierte a lenguaje maquina antes de correr el programa

En Python se usa la secuencia de Literal, Operador, Literal.

```Python code
>>> 3+2
>>> 5/'python'
>>> 5 * 'Platzi'
>>> print('Hola, Mundo')
```

#### Objetos Expresiones y tipos numéricos

**Objetos:** Son la bastraccion mas alta en programación, es la forma en la que modelamos el mundo en nuestros programas. Son valores en memoria que podemos referenciarlos con algún tipo de variable.

Tienen tipos (enteros, flotantes, booleanos, vectores), Escalares (los podemos subdividir) y no escalares (No lo podemos dividir)

```Python
# Expresion en cualquier lenguaje de programacion
#<objeto> <operador> <objeto>
x + 4
```

Las expresiones nos regresan un valor

type() Nos regresa el tipo de la variable

### 06 Asignacion de Variables

Las variables son nombres que se vinculan con un valor en memoria.

En programación se realizan asignaciones (con el símbolo’=’) a los valores que se quieren guardar en memoria , se recomienda realizar esas asignaciones con un nombre especifico de lo que significa para que todos los que vean el programa sepan de que se trata, a esas asignaciones se les llama variables, y esas variables tienen unas reglas especificas en cada lenguaje de programación.

En Python las variables pueden contener mayúsculas, minúsculas, números(sin comenzar con numero o caracter salvo _ o __ ), y no pueden llamarse como las palabras reservadas que tiene el lenguaje de programación que se esta utilizando.

Las variables hacen los programas mas comprensibles.

### 07 Cadenas y Entradas

String (tipo no escalar) son secuencias de caracteres.

```Python
>>> '123'
'123'
>>> '123'*3
'123123123'
>>> '123'+'456'
'123456'
>>> ('Hip'*3)+' '+'hurra'
'HipHipHip hurra'
>>> f'{"Hip"*3}hurra'
'HipHipHiphurra'

#utilizando Fstrings
>>> f'{"Hip"*3} hurra'
'HipHipHip hurra'
>>>
```

Operaciones con cadenas

*len
*index
*slices

#### Canedas(Strings)

* Pueden representarse con " " o ' '.

* EL operador + tiene diferente significado segun el tipo de dato (overloaded). Con cadenas significa concatenacion.

* El operador * significa de repeticion de cadenas

* Las cadenas son inmutables (siempre apuntan al mismo espacio en memoria)

##### Entradas (inputs)

* Python tiene la funcion input para recibir datos del usuario del programa.

* Input siempre regresa cadenas, por lo que si queremos utilizar otro tipo, tenemos que hacer *type casting* (convertir el string a otro tipo number('2')).

### 08 Programas Ramificados

* Repaso de los operadores de comparacion
* Reparaso de los operadores boooleanos

```python
if 5 <= 10:
    ...
elif 4 < 5:

else:
    ...
```

```python
num_1 = int(input('Escoge un entero: '))
num_2 = int(input('Escoge otro entero: '))

if num_1 > num_2:
    print('El primer numero es mayor que el segundo')
elif num_1 < num_2:
    print('El primer numero es menor que el segundo')
else:
    print('Los dos numeros son iguales')
```

Reto: Escribe un programa que compare las edades de dos usuarios y te diga quien es mayor, debe preguntarte el nombre de los usuarios.

### 10 Iteraciones

* La mayoria de las tareas computacionales no se pueden lograr con ramificaciones.
* LCuando queremos que un programa haga lo mismo varias veces, utilizamos iteraciones.
* Se pueden escribir iteraciones dentro de iteraciones.
* Podemos utilizar *break* para salir anticipadamente de una iteracion.
* Tener cuidado de iteraciones infinitas.


```python
contador_externo = 0
contador_interno = 0
while contador_externo < 5:
    while contador_interno < 6:
        print(contador_externo, contador_interno)
        contador_interno += 1

        if contador_interno >= 3:
            break

    contador_externo +=1
    contador_interno = 0
```

### 11  Bucles for

Los bucles, en diversos lenguajes de programación pueden ser definidos o indefinidos. Los bucles definidos preestablecen las condiciones de la iteración por adelantado. Por su parte, los bucles indefinidos establecen la condición en la que una iteración terminará. En este último tipo de bucles existe el riesgo de que el bucle se vuelva infinito (cuando la condición de suspensión nunca se cumple).

Los bucles definidos se implementan en Python a través del keyword for. Por su parte, los bucles indefinidos se implementan con el keyword while.

Sin embargo, esta no es la única forma de implementar bucles definidos. Por ejemplo, Javascript puede implementar un bucle definido mediante el siguiente constructo:

```javascript
for (i = 0; i <= 10; i++) {
  <expresión>
}
```

El bucle se puede leer de la siguiente manera:

Inicializa el bucle en 0
Continua el bucle mientras i sea menor o igual que 10
Incrementa i en uno al final de cada iteración
Es importante señalar que la expresión `i++` es equivalente a lo que en Python escribiríamos como `i += 1`.

Una segunda forma de crear un bucle definido es iterando en una colección de objetos. Esta es la forma que Python utiliza:

```python
for <variable> in <iterable>:
    <expresión>
```

#### El bucle for en Python

En la definición anterior debemos entender `<iterable>` como una colección de objetos; y la `<variable>` como el elemento específico que se está exponiendo mediante el bucle en cada iteración.

```Python
>>> frutas = ['manzana', 'pera', 'mango']
>>> for fruta in frutas:
        print(fruta)

manzana
pera
mango
```

**Iterables**
En Python, un iterable es un objeto que se puede utilizar en un bucle definido. Si un objeto es iterable significa que se puede pasar como argumento a la función iter. El iterable que se pasa como parámetro a la función iter
regresa un iterator.

```python
>>> iter('cadena') # cadena
>>> iter(['a', 'b', 'c']) # lista
>>> iter(('a', 'b', 'c')) # tupla
>>> iter({'a', 'b', 'c'}) # conjunto
>>> iter({'a': 1, 'b': 2, 'c': 3}) # diccionario
```

Todas las llamadas anteriores regresan un objeto de tipo iterator.

¿Qué pasa si le pasamos a la función iter un objeto que no en iterable? Obtendremos un TypeError que señala que el objeto no es un iterable. Esto es un ejemplo de programación defensiva en el que Python verifica el tipo del
objeto antes de proceder al cómputo. ¡Intentalo en tu consola!

Es importante señalar que estos no son los únicos tipos de objetos que pueden ser iterable. Existen gran cantidad de ejemplos en la librería estándar y, de hecho, casi cualquier objeto se puede convertir en un iterable (pero eso
ya lo veremos cuando hablemos de Python avanzado).

**Iterators**
Ahora que ya sabemos cómo obtener un iterator, ¿Qué podemos hacer con él? Un iterator es un objeto que regresa sucesivamente los valores asociados con el iterable.

```python
>>> frutas = ['manzana', 'pera', 'mango']
>>> iterador = iter(frutas)
>>> next(iterador)
manzana
>>> next(iterador)
pera
>>> next(iterador)
mango
```

Como puedes ver, el `iterator` guarda el estado interno de la iteración, de tal manera que cada llamada sucesiva a `next` regresa el siguiente elemento. ¿Qué pasa una vez que ya no existan más elementos en el iterable? La llamada
a next arrojará un error de tipo `StopIteration`.

```python
>>> x = iter('cadena')
>>> next(x)
'c'
>>> next(x)
'a'
>>> next(x)
'd'
>>> next(x)
'e'
>>> next(x)
'n'
>>> next(x)
'a'
>>> next(x)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
StopIteration
>>> next(x)
```

#### Cómo implementa Python los bucles definidos

Ahora ya conocemos todos los elementos necesarios para entender que es lo que sucede en Python cuando ejecutamos un bucle for. Considera nuevamente el siguiente código:

```python
>>> frutas = ['manzana', 'pera', 'mango']
>>> for fruta in frutas:
        print(fruta)
```

Este bucle se puede describir con los conceptos que explicamos previamente:

1.- Python llama internamente la función `iter` para obtener un `iterator`
2.- Una vez que tiene un iterator llama repetidamente la función `next` para
tener acceso al siguiente elemento en el bucle.
3.- Detiene el bucle una vez que se arroja el error `StopIteration`.

#### Bucles for con diccionarios

Para iterar a lo largo de un diccionario tenemos varias opciones:

* Ejecutar el bucle `for` directamente en el diccionario, lo cual nos permite
iterar a lo largo de las `llaves del diccionario`.

* Ejecutar el bucle `for` en la llamada `keys del diccionario`, lo cual nos permite
iterar a lo largo de las `llaves del diccionario`.

* Ejecutar el bucle `for` en la llamada `values` del diccionario, lo cual nos
permite iterar a lo largo de los valores del diccionario.

* Ejecutar el bucle `for` en la llamada `items` del diccionario, lo cual nos
permite iterar en una tupla de las llaves y los valores del diccionario.

```python
estudiantes = {
  'mexico': 10,
  'colombia': 15,
  'puerto_rico': 4
}


print(iter(estudiantes))
for pais in estudiantes:
  print(pais)
""" 
mexico
colombia
puerto_rico 
"""

for pais in estudiantes.keys():
  print(pais)
""" 
mexico
colombia
puerto_rico 
"""


for numero_estudiantes in estudiantes.values():
  print(numero_estudiantes)
""" 
10
15
4
"""

for pais, numero_estudiantes in estudiantes.items():
  print(pais, numero_estudiantes)
""" 
mexico 10
colombia 15
puerto_rico 4
 """
```

#### Modificación del comportamiento de un bucle for

Podemos modificar el comportamiento de un bucle for mediante los keywords
`break` y `continue`.

`break` termina el bucle y permite continuar con el resto del flujo de nuestro
programa.

`continue` termina la iteración en curso y continua con el siguiente ciclo de
iteración.

#### Conclusiones

Como pudimos observar, Python implementa los bucles definidos mediante los bucles for. Esta implementación nos permite iterar a lo largo de cualquier objeto que sea iterable. Para iterar necesitamos un iterador que nos regresará
el siguiente valor en cada iteración. Todo esto, Python lo puede hacer por nosotros con el constructo `for` ... `in` ....

## Programas numéricos

### Representación de flotantes

La mayoría del tiempo los números flotantes (tipo float) son una muy buena aproximación de los números que queremos calcular con nuestras computadoras. Sin embargo, “la mayoría del tiempo” no significa todo el tiempo, y cuando no se comportan de esta manera puede tener consecuencias inesperadas.

Por ejemplo, trata de correr el siguiente código:

```python
x = 0.0
for i in range(10):
    x += 0.1

if x == 1.0:
    print(f'x = {x}')
else:
    print(f'x != {x}')
```

Es probable que te hayas sorprendido con el resultado. La mayoría de nosotros esperaríamos que imprimiera 1.0 en vez de 0.999999999999. ¿Qué es lo que pasó?.

Para entender qué es lo que pasó tenemos que entender que es lo que pasa en la computadora cuando realizamos cómputos con números flotantes. Y para eso necesitamos entender números binarios.

Cuando aprendiste a contar, lo que en realidad aprendiste es una técnica combinatoria para manipular los siguientes símbolos que le llamamos números: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9.

La forma en la que funciona esta técnica es asignando el número 10 a la 0 al número de la extrema derecha, 10 a la 1 al siguiente, 10 a la 2 al siguiente y así sucesivamente. De tal manera que el número 525 es simplemente la representación de `(5 * 100) + (2 * 10) + (5 * 1)`.

Esto nos dice que el número de números que podemos representar depende de cuanto espacio tengamos. Si tenemos un espacio de 3, podemos representar 1,000 números (10 elevado a la 3) o la secuencia del 0 al 999. Si tenemos 4, podemos representar 10,000 (10 elevado a la 4) o la secuencia del 0 al 9,999. De manera general podemos decir que con una secuencia de tamaño n, podemos representar 10 elevado a la n números.

Los números binarios funcionan de la misma manera (de hecho cualquier número en cualquier base, por ejemplo, octales o hexadecimales). La única diferencia es cuántos símbolos tenemos para representar. En binario nada más tenemos 0, 1;
en hexadecimal tenemos 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e, f.

De esta manera podemos decir que el número de la extrema derecha es cantidad_de_simbolos**0, cantidad_de_simbolos**1, cantidad_de_simbolos**2, etc. Por lo que en binario, que nada más tenemos 2 símbolos, decimos 2**0, 2**1, 2**2, etc. Por ejemplo el número binario 101 es la representación de `(1 * 4) + (0 * 2) + (1 * 1)`, es decir 5.

Esta representación nos permite trabajar con todos los números positivos enteros dentro del computador, pero ¿Qué hacemos con los negativos y los racionales?.

El caso de los números negativos es sencillo: simplemente agregamos un bit adicional que representa el signo y la añadimos en la extrema izquierda. Por lo que el número 0101 sería +5 y el número 1101 sería -5.

El caso de los racionales es más complejo. En la mayoría de los lenguajes de programación modernos los racionales utilizan una implementación llamada punto flotante. ¿Cómo funciona esta representación?.

Antes de pasar a binario, vamos a pretender que estamos trabajando con una computadora basada en decimales. Un número flotante lo representaríamos con un par de enteros: los dígitos significativos y el exponente. Por ejemplo, el número 2.345 se representaría como (2345 * 10**-3) o (2345, -3).

El número de dígitos significativos determinan la precisión con la que podemos representar número. Por ejemplo si nada más tuviéramos dos dígitos significativos el número 2.345 no se podría representar de manera exacta y tendríamos que convertirlo a una aproximación, en este caso 2.3.

Ahora pasemos a la verdadera representación interna de la computadora, que es en binario. ¿Cómo representarías el número 5/8 o 0.625? Lo primero que tenemos que saber es que 5/8 es en realidad el número 5 * 2**-3. Por lo que podríamos decir (101, -11) (recuerda que el número 5 es 101 en binario y el 3 es 11).

Regresemos a nuestro problema inicial: ¿Cómo representaremos 1/10 (que escribimos en Python cómo 0.1)? Lo mejor que podemos hacer con cuatro dígitos significativos es (0011, -101) que es equivalente a 3/32 (0.09375). ¿Qué tal si tuviéramos cinco dígitos significativos? La mejor representación sería (11001, -1000) que es equivalente a 25/256 (0.09765625). ¿Cuántos dígitos significativos necesitamos entonces? Un número infinito. No existe ningún número que cumpla con la siguiente ecuación: sim * 2**-exp.

En la mayoría de las implementaciones de Python tenemos 53 bits de precisión para números flotantes. Así que los dígitos significativos para representar el número 0.1 es igual a:

11001100110011001100110011001100110011001100110011001 que es equivalente al número decimal: 0.1000000000000000055511151231257827021181583404541015625

Muy cercano a 1/10 pero no exactamente 1/10. Ahora ya sabemos la razón de esa respuesta tan extraña. Hay muy pocas situaciones en la que 1.0 es aceptable, pero 0.9999999999999999 no. Pero ¿Cuál es la moraleja de esta historia?

Hasta ahora hemos verificado igualdad con el operador ==. Sin embargo, cuando estamos trabajando con flotantes es mejor asegurarnos que los números sean aproximados en vez de idénticos. Por ejemplo x < 1.0 and x > 0.99999.

### Enumeracion exhaustiva

* Tambien llamado "adivina y verifica"
* Las computadoras actuales son muy muy rapidas
* Uno de los primeros algoritmos que debes tratar

```py
'saber si un numero tiene una raiz exacta'

objetivo = int(input('Escoge un entero: '))
respuesta = 0

while respuesta**2 < objetivo:
    print(respuesta)
    respuesta += 1

if respuesta**2 == objetivo:
    print(f'La raiz cuadrada de  {objetivo} es {respuesta}')
else:
    print(f'{objetivo} no tiene una raiz cuadrada exacta')
```

### 14 Aproximacion de Soluciones

* Similar a enumeracion exhaustiva, pero no necesita una respuesta exacta.
* Podemos aproximar soluciones con un margen de error que llamaremos epsilon
  
Entre mas preciso mas iteraciones sera necesarias

```py
objetivo = int(input('Escoge un entero: '))
epsilon = 0.01
paso = epsilon**2
respuesta = 0.0

while abs(respuesta**2 - objetivo) >= epsilon and respuesta <= objetivo:
    # print(abs(respuesta**2 - objetivo), respuesta)
    respuesta += paso

if abs(respuesta**2 - objetivo) >= epsilon:
    print(f'No se encontro la raiz cuadrada {objetivo}')
else:
    print(f'La raiz cuadrada {objetivo} es {respuesta}')
```

### 15 Busqueda Binaria

* Cuando la respuesta se encuentra en una conjunto ordenado, podemos utilizar busqueda binaria.

* Es altamente eficiente, pues acorda el espacio de busqueda en dos por cada iteracion.

```py
# Introducción al Pensamiento Computacional con Python 

## Modulo I Introduccion al pensamiento computacional

### 01 Introduccion al pensamiento computacional

Breve introduccion de david aroestti sobre para que sirve programar y los usos que el le da a python en su vida diaria laboral

### 02 Introduccion al computo

* El telar de jackart incorporo el computo con punch-cards.

* Motor Analitico de babage, crea una maquina general que podia manejar calculos usando engranes.

* Un problema que resolvio las computadoras fue el censo de estados unidos.

* A final de los 30 Alan Turing y Alonso Church vienen con la maquina imaginaria de la cinta infinita, todos los algoritomos que tenemos como humanidad era la misma secuencia de instrucciones se puede computar matematicamente.

* ENIAC se construye para programarse con cables

* Von Neuman genera la primer computadora donde puedes insertar un programa

* Richard Fayman nos da las bases matematicas para el computo cuantico.

#### Computo y Computadoras

* Las computadoras hacen dos cosas: hacen calculos y recuerdan el resultado de dichos calculos

* Aun con las computadoras modernas existen problemas que no podemos resolver.

### 03 Introduccion a los lenguajes de programacion

#### Conocimiento declarativo vs imperativo

**Declarativo:** nos dice que tipo de relaciones existe entre ciertas variables, entre diersos objetos.

**Impertativo:** nos dice como lograr un objetivo

**Algoritmo:** "Un algoritmo es una lista finita de instrucciones que describen un computo, que cuando se ejecuta con ciertas entradas (inputs) ejectuta pasos intermedios para llegar a un resultado (output)" *John V. Guttag*

Los lenguajes de programacion nacen con ada lovelace, mientras los de alto nivel llegan con Grace Hopper.

##### Programacion

* **Turing completeness**: implementan todos los primitivos que en principio necesitamos para hacer cualquier tipo de algoritmo.

* Los lenguajes de programacion modernos dan primitivos que son mas convenientes que los primitivos de Turing.

##### Lenguajes( Son precisos, exactos, y tienen un solo significado, no son ambuguos)

* **Sintaxis:** Defne al secuencia de simbolos que esta bien formada.

* **Semantica estatica:** Define que eninciados con sintaxis correcta tienen significado.

* **Semantica:** Define el significado. En los lenguajes de programacion solo hay un significado.

## Modulo II Introducción a Python

### 04 Preparacion de tu computadora

Realizamos la configuracion basica para integrar python a tu sistema operativo e instalamos VSCode.

### 05 Elementos Basicos de Python

#### Lenguajes de programacion
No vamos a Aprender python sino que se hablará de los elementos básicos de programación

**Alto nivel:** está diseñado para los humanos. *Pyrthon
**Bajo nivel:** Está optimizado para las computadoras, se acerca mas a los 1/0
**General:**  Que tiene todos los primitivos que nos otorga Turing para poder implementar algoritmos. 
**Dominio Específico:** Están dirigidos hacia aplicaciones muy específicas
**Interpretados:** Mientras correo el programa , después de cada instrucción esta es leída por el programa.
**Compilado:** Se convierte a lenguaje maquina antes de correr el programa

En Python se usa la secuencia de Literal, Operador, Literal.

```Python code
>>> 3+2
>>> 5/'python'
>>> 5 * 'Platzi'
>>> print('Hola, Mundo')
```

#### Objetos Expresiones y tipos numéricos

**Objetos:** Son la bastraccion mas alta en programación, es la forma en la que modelamos el mundo en nuestros programas. Son valores en memoria que podemos referenciarlos con algún tipo de variable.

Tienen tipos (enteros, flotantes, booleanos, vectores), Escalares (los podemos subdividir) y no escalares (No lo podemos dividir)

```Python
# Expresion en cualquier lenguaje de programacion
#<objeto> <operador> <objeto>
x + 4
```

Las expresiones nos regresan un valor

type() Nos regresa el tipo de la variable

### 06 Asignacion de Variables

Las variables son nombres que se vinculan con un valor en memoria.

En programación se realizan asignaciones (con el símbolo’=’) a los valores que se quieren guardar en memoria , se recomienda realizar esas asignaciones con un nombre especifico de lo que significa para que todos los que vean el programa sepan de que se trata, a esas asignaciones se les llama variables, y esas variables tienen unas reglas especificas en cada lenguaje de programación.

En Python las variables pueden contener mayúsculas, minúsculas, números(sin comenzar con numero o caracter salvo _ o __ ), y no pueden llamarse como las palabras reservadas que tiene el lenguaje de programación que se esta utilizando.

Las variables hacen los programas mas comprensibles.

### 07 Cadenas y Entradas

String (tipo no escalar) son secuencias de caracteres.

```Python
>>> '123'
'123'
>>> '123'*3
'123123123'
>>> '123'+'456'
'123456'
>>> ('Hip'*3)+' '+'hurra'
'HipHipHip hurra'
>>> f'{"Hip"*3}hurra'
'HipHipHiphurra'

#utilizando Fstrings
>>> f'{"Hip"*3} hurra'
'HipHipHip hurra'
>>>
```

Operaciones con cadenas

*len
*index
*slices

#### Canedas(Strings)

* Pueden representarse con " " o ' '.

* EL operador + tiene diferente significado segun el tipo de dato (overloaded). Con cadenas significa concatenacion.

* El operador * significa de repeticion de cadenas

* Las cadenas son inmutables (siempre apuntan al mismo espacio en memoria)

##### Entradas (inputs)

* Python tiene la funcion input para recibir datos del usuario del programa.

* Input siempre regresa cadenas, por lo que si queremos utilizar otro tipo, tenemos que hacer *type casting* (convertir el string a otro tipo number('2')).

### 08 Programas Ramificados

* Repaso de los operadores de comparacion
* Reparaso de los operadores boooleanos

```python
if 5 <= 10:
    ...
elif 4 < 5:

else:
    ...
```

```python
num_1 = int(input('Escoge un entero: '))
num_2 = int(input('Escoge otro entero: '))

if num_1 > num_2:
    print('El primer numero es mayor que el segundo')
elif num_1 < num_2:
    print('El primer numero es menor que el segundo')
else:
    print('Los dos numeros son iguales')
```

Reto: Escribe un programa que compare las edades de dos usuarios y te diga quien es mayor, debe preguntarte el nombre de los usuarios.

### 10 Iteraciones

* La mayoria de las tareas computacionales no se pueden lograr con ramificaciones.
* LCuando queremos que un programa haga lo mismo varias veces, utilizamos iteraciones.
* Se pueden escribir iteraciones dentro de iteraciones.
* Podemos utilizar *break* para salir anticipadamente de una iteracion.
* Tener cuidado de iteraciones infinitas.


```python
contador_externo = 0
contador_interno = 0
while contador_externo < 5:
    while contador_interno < 6:
        print(contador_externo, contador_interno)
        contador_interno += 1

        if contador_interno >= 3:
            break

    contador_externo +=1
    contador_interno = 0
```

### 11  Bucles for

Los bucles, en diversos lenguajes de programación pueden ser definidos o indefinidos. Los bucles definidos preestablecen las condiciones de la iteración por adelantado. Por su parte, los bucles indefinidos establecen la condición en la que una iteración terminará. En este último tipo de bucles existe el riesgo de que el bucle se vuelva infinito (cuando la condición de suspensión nunca se cumple).

Los bucles definidos se implementan en Python a través del keyword for. Por su parte, los bucles indefinidos se implementan con el keyword while.

Sin embargo, esta no es la única forma de implementar bucles definidos. Por ejemplo, Javascript puede implementar un bucle definido mediante el siguiente constructo:

```javascript
for (i = 0; i <= 10; i++) {
  <expresión>
}
```

El bucle se puede leer de la siguiente manera:

Inicializa el bucle en 0
Continua el bucle mientras i sea menor o igual que 10
Incrementa i en uno al final de cada iteración
Es importante señalar que la expresión `i++` es equivalente a lo que en Python escribiríamos como `i += 1`.

Una segunda forma de crear un bucle definido es iterando en una colección de objetos. Esta es la forma que Python utiliza:

```python
for <variable> in <iterable>:
    <expresión>
```

#### El bucle for en Python

En la definición anterior debemos entender `<iterable>` como una colección de objetos; y la `<variable>` como el elemento específico que se está exponiendo mediante el bucle en cada iteración.

```Python
>>> frutas = ['manzana', 'pera', 'mango']
>>> for fruta in frutas:
        print(fruta)

manzana
pera
mango
```

**Iterables**
En Python, un iterable es un objeto que se puede utilizar en un bucle definido. Si un objeto es iterable significa que se puede pasar como argumento a la función iter. El iterable que se pasa como parámetro a la función iter
regresa un iterator.

```python
>>> iter('cadena') # cadena
>>> iter(['a', 'b', 'c']) # lista
>>> iter(('a', 'b', 'c')) # tupla
>>> iter({'a', 'b', 'c'}) # conjunto
>>> iter({'a': 1, 'b': 2, 'c': 3}) # diccionario
```

Todas las llamadas anteriores regresan un objeto de tipo iterator.

¿Qué pasa si le pasamos a la función iter un objeto que no en iterable? Obtendremos un TypeError que señala que el objeto no es un iterable. Esto es un ejemplo de programación defensiva en el que Python verifica el tipo del
objeto antes de proceder al cómputo. ¡Intentalo en tu consola!

Es importante señalar que estos no son los únicos tipos de objetos que pueden ser iterable. Existen gran cantidad de ejemplos en la librería estándar y, de hecho, casi cualquier objeto se puede convertir en un iterable (pero eso
ya lo veremos cuando hablemos de Python avanzado).

**Iterators**
Ahora que ya sabemos cómo obtener un iterator, ¿Qué podemos hacer con él? Un iterator es un objeto que regresa sucesivamente los valores asociados con el iterable.

```python
>>> frutas = ['manzana', 'pera', 'mango']
>>> iterador = iter(frutas)
>>> next(iterador)
manzana
>>> next(iterador)
pera
>>> next(iterador)
mango
```

Como puedes ver, el `iterator` guarda el estado interno de la iteración, de tal manera que cada llamada sucesiva a `next` regresa el siguiente elemento. ¿Qué pasa una vez que ya no existan más elementos en el iterable? La llamada
a next arrojará un error de tipo `StopIteration`.

```python
>>> x = iter('cadena')
>>> next(x)
'c'
>>> next(x)
'a'
>>> next(x)
'd'
>>> next(x)
'e'
>>> next(x)
'n'
>>> next(x)
'a'
>>> next(x)
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
StopIteration
>>> next(x)
```

#### Cómo implementa Python los bucles definidos

Ahora ya conocemos todos los elementos necesarios para entender que es lo que sucede en Python cuando ejecutamos un bucle for. Considera nuevamente el siguiente código:

```python
>>> frutas = ['manzana', 'pera', 'mango']
>>> for fruta in frutas:
        print(fruta)
```

Este bucle se puede describir con los conceptos que explicamos previamente:

1.- Python llama internamente la función `iter` para obtener un `iterator`
2.- Una vez que tiene un iterator llama repetidamente la función `next` para
tener acceso al siguiente elemento en el bucle.
3.- Detiene el bucle una vez que se arroja el error `StopIteration`.

#### Bucles for con diccionarios

Para iterar a lo largo de un diccionario tenemos varias opciones:

* Ejecutar el bucle `for` directamente en el diccionario, lo cual nos permite
iterar a lo largo de las `llaves del diccionario`.

* Ejecutar el bucle `for` en la llamada `keys del diccionario`, lo cual nos permite
iterar a lo largo de las `llaves del diccionario`.

* Ejecutar el bucle `for` en la llamada `values` del diccionario, lo cual nos
permite iterar a lo largo de los valores del diccionario.

* Ejecutar el bucle `for` en la llamada `items` del diccionario, lo cual nos
permite iterar en una tupla de las llaves y los valores del diccionario.

```python
estudiantes = {
  'mexico': 10,
  'colombia': 15,
  'puerto_rico': 4
}


print(iter(estudiantes))
for pais in estudiantes:
  print(pais)
""" 
mexico
colombia
puerto_rico 
"""

for pais in estudiantes.keys():
  print(pais)
""" 
mexico
colombia
puerto_rico 
"""


for numero_estudiantes in estudiantes.values():
  print(numero_estudiantes)
""" 
10
15
4
"""

for pais, numero_estudiantes in estudiantes.items():
  print(pais, numero_estudiantes)
""" 
mexico 10
colombia 15
puerto_rico 4
 """
```

#### Modificación del comportamiento de un bucle for

Podemos modificar el comportamiento de un bucle for mediante los keywords
`break` y `continue`.

`break` termina el bucle y permite continuar con el resto del flujo de nuestro
programa.

`continue` termina la iteración en curso y continua con el siguiente ciclo de
iteración.

#### Conclusiones

Como pudimos observar, Python implementa los bucles definidos mediante los bucles for. Esta implementación nos permite iterar a lo largo de cualquier objeto que sea iterable. Para iterar necesitamos un iterador que nos regresará
el siguiente valor en cada iteración. Todo esto, Python lo puede hacer por nosotros con el constructo `for` ... `in` ....

## Programas numéricos

### Representación de flotantes

La mayoría del tiempo los números flotantes (tipo float) son una muy buena aproximación de los números que queremos calcular con nuestras computadoras. Sin embargo, “la mayoría del tiempo” no significa todo el tiempo, y cuando no se comportan de esta manera puede tener consecuencias inesperadas.

Por ejemplo, trata de correr el siguiente código:

```python
x = 0.0
for i in range(10):
    x += 0.1

if x == 1.0:
    print(f'x = {x}')
else:
    print(f'x != {x}')
```

Es probable que te hayas sorprendido con el resultado. La mayoría de nosotros esperaríamos que imprimiera 1.0 en vez de 0.999999999999. ¿Qué es lo que pasó?.

Para entender qué es lo que pasó tenemos que entender que es lo que pasa en la computadora cuando realizamos cómputos con números flotantes. Y para eso necesitamos entender números binarios.

Cuando aprendiste a contar, lo que en realidad aprendiste es una técnica combinatoria para manipular los siguientes símbolos que le llamamos números: 0, 1, 2, 3, 4, 5, 6, 7, 8, 9.

La forma en la que funciona esta técnica es asignando el número 10 a la 0 al número de la extrema derecha, 10 a la 1 al siguiente, 10 a la 2 al siguiente y así sucesivamente. De tal manera que el número 525 es simplemente la representación de `(5 * 100) + (2 * 10) + (5 * 1)`.

Esto nos dice que el número de números que podemos representar depende de cuanto espacio tengamos. Si tenemos un espacio de 3, podemos representar 1,000 números (10 elevado a la 3) o la secuencia del 0 al 999. Si tenemos 4, podemos representar 10,000 (10 elevado a la 4) o la secuencia del 0 al 9,999. De manera general podemos decir que con una secuencia de tamaño n, podemos representar 10 elevado a la n números.

Los números binarios funcionan de la misma manera (de hecho cualquier número en cualquier base, por ejemplo, octales o hexadecimales). La única diferencia es cuántos símbolos tenemos para representar. En binario nada más tenemos 0, 1;
en hexadecimal tenemos 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e, f.

De esta manera podemos decir que el número de la extrema derecha es cantidad_de_simbolos**0, cantidad_de_simbolos**1, cantidad_de_simbolos**2, etc. Por lo que en binario, que nada más tenemos 2 símbolos, decimos 2**0, 2**1, 2**2, etc. Por ejemplo el número binario 101 es la representación de `(1 * 4) + (0 * 2) + (1 * 1)`, es decir 5.

Esta representación nos permite trabajar con todos los números positivos enteros dentro del computador, pero ¿Qué hacemos con los negativos y los racionales?.

El caso de los números negativos es sencillo: simplemente agregamos un bit adicional que representa el signo y la añadimos en la extrema izquierda. Por lo que el número 0101 sería +5 y el número 1101 sería -5.

El caso de los racionales es más complejo. En la mayoría de los lenguajes de programación modernos los racionales utilizan una implementación llamada punto flotante. ¿Cómo funciona esta representación?.

Antes de pasar a binario, vamos a pretender que estamos trabajando con una computadora basada en decimales. Un número flotante lo representaríamos con un par de enteros: los dígitos significativos y el exponente. Por ejemplo, el número 2.345 se representaría como (2345 * 10**-3) o (2345, -3).

El número de dígitos significativos determinan la precisión con la que podemos representar número. Por ejemplo si nada más tuviéramos dos dígitos significativos el número 2.345 no se podría representar de manera exacta y tendríamos que convertirlo a una aproximación, en este caso 2.3.

Ahora pasemos a la verdadera representación interna de la computadora, que es en binario. ¿Cómo representarías el número 5/8 o 0.625? Lo primero que tenemos que saber es que 5/8 es en realidad el número 5 * 2**-3. Por lo que podríamos decir (101, -11) (recuerda que el número 5 es 101 en binario y el 3 es 11).

Regresemos a nuestro problema inicial: ¿Cómo representaremos 1/10 (que escribimos en Python cómo 0.1)? Lo mejor que podemos hacer con cuatro dígitos significativos es (0011, -101) que es equivalente a 3/32 (0.09375). ¿Qué tal si tuviéramos cinco dígitos significativos? La mejor representación sería (11001, -1000) que es equivalente a 25/256 (0.09765625). ¿Cuántos dígitos significativos necesitamos entonces? Un número infinito. No existe ningún número que cumpla con la siguiente ecuación: sim * 2**-exp.

En la mayoría de las implementaciones de Python tenemos 53 bits de precisión para números flotantes. Así que los dígitos significativos para representar el número 0.1 es igual a:

11001100110011001100110011001100110011001100110011001 que es equivalente al número decimal: 0.1000000000000000055511151231257827021181583404541015625

Muy cercano a 1/10 pero no exactamente 1/10. Ahora ya sabemos la razón de esa respuesta tan extraña. Hay muy pocas situaciones en la que 1.0 es aceptable, pero 0.9999999999999999 no. Pero ¿Cuál es la moraleja de esta historia?

Hasta ahora hemos verificado igualdad con el operador ==. Sin embargo, cuando estamos trabajando con flotantes es mejor asegurarnos que los números sean aproximados en vez de idénticos. Por ejemplo x < 1.0 and x > 0.99999.

### Enumeracion exhaustiva

* Tambien llamado "adivina y verifica"
* Las computadoras actuales son muy muy rapidas
* Uno de los primeros algoritmos que debes tratar

```py
'saber si un numero tiene una raiz exacta'

objetivo = int(input('Escoge un entero: '))
respuesta = 0

while respuesta**2 < objetivo:
    print(respuesta)
    respuesta += 1

if respuesta**2 == objetivo:
    print(f'La raiz cuadrada de  {objetivo} es {respuesta}')
else:
    print(f'{objetivo} no tiene una raiz cuadrada exacta')
```

### 14 Aproximacion de Soluciones

* Similar a enumeracion exhaustiva, pero no necesita una respuesta exacta.
* Podemos aproximar soluciones con un margen de error que llamaremos epsilon
  
Entre mas preciso mas iteraciones sera necesarias

```py
objetivo = int(input('Escoge un entero: '))
epsilon = 0.01
paso = epsilon**2
respuesta = 0.0

while abs(respuesta**2 - objetivo) >= epsilon and respuesta <= objetivo:
    # print(abs(respuesta**2 - objetivo), respuesta)
    respuesta += paso

if abs(respuesta**2 - objetivo) >= epsilon:
    print(f'No se encontro la raiz cuadrada {objetivo}')
else:
    print(f'La raiz cuadrada {objetivo} es {respuesta}')
```

### 15 Busqueda Binaria

* Cuando la respuesta se encuentra en una conjunto ordenado, podemos utilizar busqueda binaria.

* Es altamente eficiente, pues acorda el espacio de busqueda en dos por cada iteracion.

```py
objetivo = int(input('Escoge un entero: '))
epsilon = 0.00001
bajo = 0.0
alto = max(1.0, objetivo)
respuesta = (alto + bajo) / 2

while abs(respuesta**2 - objetivo) >= epsilon:
    if respuesta**2 < objetivo:
        bajo = respuesta
    else:
        alto = respuesta

    respuesta = (alto + bajo) / 2

print(f'La raiz cuadrada del {objetivo} es la {respuesta}')
```

## IV Funciones, alcance y abstracción

### 16 Funciones y abstracción

Abstraccion: tu no necesitas entender como algo funciona internamente para poderlo operar (e.g. calculadora)

Decomposicion:

* Permite dividir el codigo en componentes que colaboran con un fin en comun

* Se puede pensar como mini programas dentro de un programa mayor.

```py
def <nombre> (<parametros>):
    <cuerpo>
    return <expresion>

def suma(a,b):
  total = a + b
  return total

suma(2,3)
```

Las funciones en python pueden tener argumentos de tipo keyword o valores por defecto (**kawrgs)

```py
def nombre_completo(nombre, apellido, inverso=False):
  if inverso:
    return f'{apellido} {nombre}'
  else:
    return f'{nombre} {apellido}'

nombre_completo('David', 'Aroesti')
nombre_completo('David', 'Aroesti', inverso=True)
nombre_completo('David', 'Aroesti', inverso=True)
nombre_completo(apellido='Aroesti', nombre='David')
```

Reto Solucion

```py
def enumeracion_exahustiva():
    objetivo = int(input('Escoge un entero: '))
    epsilon = 0.01
    paso = epsilon**2
    respuesta = 0.0

    while abs(respuesta**2 - objetivo) >= epsilon and respuesta <= objetivo:
        # print(abs(respuesta**2 - objetivo), respuesta)
        respuesta += paso

    if abs(respuesta**2 - objetivo) >= epsilon:
        print(f'No se encontro la raiz cuadrada {objetivo}')
    else:
        print(f'La raiz cuadrada {objetivo} es {respuesta}')

if 'name' == '__main__'
    enumeracion_exahustiva()
```

### 17 Scope o Alcance

```py
def func1(un_arg, una_func):
  def func2(otro_arg):
    return otro_arg * 2

  valor = func2(un_arg)
  return una_func(valor)

un_arg = 1

def cualquier_func(cualquier_arg):
return cualquier_arg + 5

func1(un_arg, cuaquier_func)
```

Los frammes son la forma en que funcionan internamente los lenguajes de programacion.


### 18 Especificacions del codigo

```py

# Suma 
def suma(a,b):
  """Suma dos valores a y b

  para int a cualquier entero
  para int ba cualquier entero
  """
  total = a + b
  return total

suma(2,3)
```

Un doscstring debe  describir tres cosas:

* Que hace la funcion.
* Que significan los parametros, cuaes son y que tipo de valor pueden ser.
* Que regresa la funcion.

Ejemplo terminal

```py
def a(cualquier_parametro):
  """ Descripcion de lo que hace nuestra funcion.

    cualquier parametro int cualquier entero
    returns cualquier_parametro + 5
  """
```

Para poder entender esto usamos la funcion help, y pasamos como parametro la funcion u objeto que del que queremos obtener la ayuda.

```py
help(a)
```

### 19 Recursividad

* Algoritmica: Una forma de  crear soluciones utilizando el principio "divide y venceras"

* Programatica: Una tecnica programatica mendiante la cual una funcion se llama a si misma.

```py
    """
    Calcula el factorial de n.
  
    n int > 0
    returns n!
    """
    print(n)
    #siempre define caso base
    if n == 1:
        return 1

    return n * factorial(n - 1)

n = int(input('Escribe un entero: '))

print(factorial(n))
```

### 20 Fibonnacci y la Recursividad

La secuencia de Fibonacci es una función matemática que se define recursivamente. En el año 1202, el matemático italiano Leonardo de Pisa, también conocido como Fibonacci, encontró una fórmula para cuantificar el crecimiento que ciertas poblaciones (como la de los conejos) experimentan.

Supón que una pareja de conejos nace, un macho y una hembra, y luego son liberados. Supón, también, que los conejos se pueden reproducir hasta la edad de un mes y que tienen un periodo de gestación de un mes. Por último supón que
estos conejos nunca mueren y que la hembra siempre es capaz de producir una nueva pareja (un macho y una hembra).¿Cuántos conejos existirán al final de seis meses?

Una forma de visualizar este crecimiento es mirándolo de forma tabular:

Mes |	Hembras
| 0	| 1 |
| 1	| 1 |
| 2	| 2 |
| 3	| 3 |
| 4	| 5 |
| 5	| 8 |
| 6	|13|

Un punto importante a considerar es que para el mes n > 1, hembras(n) = hembras(n - 1) + hembras(n - 2).

Como podemos ver, tenemos una definición distinta a la de factorial que vimos anteriormente. En específico, tenemos dos casos base (0 y 1) y tenemos dos llamadas recursivas (hembras(n - 1) + hembras(n - 2)).

Podemos crear una solución recursiva de manera sencilla:

```py
def fibonacci(n):
    if n == 0 or n == 1:
        return 1

    return fibonacci(n - 1) + fibonacci(n - 2)
```

Aunque la definición es muy sencilla, es también bastante ineficiente. En los siguientes cursos de la serie de pensamiento computacional veremos como calcular exactamente la eficiencia de este algoritmo y cómo optimizarlo.

## V Tipos estructurados, mutabilidad y funciones de alto nivel

### 21 Funciones como objetos

#### Funciones como objetos

Una de las características más poderosas de Python es que todo es un objeto, incluyendo las funciones. Las funciones en Python son “ciudadanos de primera clase”.

Esto, en sentido amplio, significa que en Python las funciones:

* Tienen un tipo
* Se pueden pasar como argumentos de otras funciones
* Se pueden utilizar en expresiones
* Se pueden incluir en varias estructuras de datos (como listas, tuplas,
diccionarios, etc.)

### Argumentos de otras funciones

Hasta ahora hemos visto que las funciones pueden recibir parámetros para realizar los cómputos que definen. Algunos de los tipos que hemos pasado son tipos simples como cadenas, números, listas, etc. Sin embargo, también pueden recibir funciones para crear abstracciones más poderosas. Veamos un ejemplo:

```py
def multiplicar_por_dos(n):
    return n * 2

def sumar_dos(n):
    return n + 2

def aplicar_operacion(f, numeros):
    resultados = []
    for numero in numeros:
        resultado = f(numero)
        resultados.append(resultado)

>>> nums = [1, 2, 3]
>>> aplicar_operacion(multiplicar_por_dos, nums)
[2, 4, 6]

>>> aplicar_operacion(sumar_dos, nums)
[3, 4, 5]
```

### Funciones en expresiones

Una forma de definir una función en una expresión es utilizando el keyword lambda. lambda tiene la siguiente sintaxis: `lambda <vars>: <expresion>`.

Otro ejemplo interesante es que las funciones se pueden utilizar en una expresión directamente. Esto es posible ya que como lo hemos platicado con anterioridad, en Python las variables son simplemente nombres que apuntan a un objeto (en este caso a una función). Por ejemplo:

```py
sumar = lambda x, y: x + y

>>> sumar(2, 3)
5
```

#### Funciones en estructuras de datos

Las funciones también se pueden incluir en diversas estructuras que las permiten almacenar. Por ejemplo, una lista puede guardar diversas funciones a aplicar o un diccionario las puede almacenar como valores.

```pydef aplicar_operaciones(num):
    operaciones = [abs, float]

    resultado = []
    for operacion in operaciones:
        resultado.append(operacion(num))

    return resultado

>>> aplicar_operaciones(-2)
[2, -2.0]
```

Como pudimos ver, las funciones son objetos muy versátiles que nos permiten tratarlas de diversas maneras y que nos permiten añadir capas adicionales de abstracción a nuestro programa.

### 22 Tuplas

* Son secuencias inmutables de objetos.
* A diferencia de las cadenas pueden contener cualquier tipo de objeto.
* Puede utilizarse para devolver varios valores en una funcion.
* Una tupla requiere indicarse con coma
* Una tupla se puede reasignar

```py
>>> my_tuple = ()
>>> type(my_tuple)
<class 'tuple'>

#Asignar
>>> my_tuple = (1,'dos', True)
>>> my_tuple[0]
1

#Inmutar
>>> my_tuple[0] = 2
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'tuple' object does not support item assignment


#Reasignar
>>> my_other_tuple = (2,3,4)
>>> my_tuple += my_other_tuple
>>> my_tuple
(1, 'dos', True, 2, 3, 4)

#Desempaquetar
>>> x,y,z = my_other_tuple
>>> x
2
>>> y
3
>>> z
4


>>> def coordenadas():
...     return (5,4)
...
>>> x, y = coordenadas()
>>> print(x,y)
5 4
>>>
```

### 23 Rangos

* Representan una secuencia de enteros
* range(comienzo,fin,pasos)
* Al igual que eas cadenas y las tupas, los rangos son inmutables
* Muy eficientes en uso de memoria normalmente utilizados en for loops
  
```py
# range(comienzo, fin, pasos)

>>> my_range = range(1,5)
>>> type(my_range)
<class 'range'>
>>> for i in my_range:
...     print(i)
...
1
2
3
4
>>> my_range = range(0,7,2)
>>> my_other_range = range(0,8,2)
>>> 
>>> 

# comparativa content equality
>>> my_range == my_other_range
True
>>> for i in my_other_range:
...     print(i)
...
0
2
4
6

>>> for i in my_range:
...     print(i)
...
0
2
4
6

# comparativa object equality (operador is)
>>> id(my_range)
140007565863648
>>> id(my_other_range)
140007565863504
>>>
>>> 
>>> my_range is my_other_range
False
```

### 24 Listas y mutabilidad

* Son secuencias de objeos pero a diferencia de las tuplas, si son mutabes.
* Cuando modificas una lista, pueden existir efectos secundarios (side effects)
* Es posible iterar con ellas.
* Para modificar una lista podemos:
  * Asignar via indice (my)lista[0]=5)
  * Utilizar los metodos de la lista (append, pop, remove, insert, etc).


```py
#crear
>>> my_list = [1,2,3]
>>> my_list 
[1, 2, 3]

# Slice notation
>>> my_list[1:]
[2, 3]

#Agregar elemento al final
>>> my_list.append(4)
>>> my_list
[1, 2, 3, 4]

#Sustituir elemento por indices
>>> my_list[0] = 'a'
>>> my_list
['a', 2, 3, 4]

# Pop, elimina y retorna elemento eliminado
>>> my_list.pop()
4
>>> my_list
['a', 2, 3]

# Iteracion
>>> for element in my_list:
...     print(element)
...
a
2
3

#Memoria 
>>> a = my_list
>>> b = a
>>> id(a)
140007565705352
>>> id(b)
140007565705352
>>>
>>> c = [a,b]
>>> c
[['a', 2, 3], ['a', 2, 3]]

# Fuentes de bugs
>>> a.append(5)
>>> c
[['a', 2, 3, 5], ['a', 2, 3, 5]]
>>>
```

#### Clonacion

* Casi siempre es mejor clonar una lista en vez de mutarla
* Para clonar una lista podemos utilizar rebanas (slices) o la funcion list

Ejemplo list


```py
>>> a = [1,2,3]
>>> b = a
>>> c = list(a)

# Diferentes objetos  a not c
... id(a)
140007565320840
>>> id(b)
140007565320840
>>> id(c)
140007565
>>> id(d)
140007565321224
>>>
```

#### List comprenhension

* Es una forma consisa de aplicar operaciones a los valores de una secuencia
* Tambien se pueden aplicar condiciones para filtrar


```py
>>> my_list = list(range(100))
>>> my_list
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 
30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99]
>>>

>>> double = [i * 2 for i in my_list]
>>> double
[0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 96, 98, 100, 102, 104, 106, 108, 110, 112, 114, 116, 118, 120, 122, 124, 126, 128, 130, 132, 134, 136, 138, 140, 142, 144, 146, 148, 150, 152, 154, 156, 158, 160, 162, 164, 166, 168, 170, 172, 174, 176, 178, 180, 182, 184, 186, 188, 190, 192, 194, 196, 198]

>>> pares = [i for i in my_list if i % 2 == 0]
>>> pares
[0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 96, 98]
>>>
```

### 25 Diccionarios

* Son como listas, pero en lugar de usar indices utilizan llaves.
* No tienen orden interno.
* Los diccionarios son mutables.
* Pueden iterarse.

Son hashmaps sin orden interno, pero con valores unicos en sus llaves (hashes).

```py
#Creacion diccionario
>>> my_dict = {
...     'David': 35,
...     'Erika': 32,
...     'Jaime': 50
... }

# Accede por indices
>>> my_dict['David']
35  

# Usa get para evitar un error cuando la llave no exista
>>> my_dict.get('Juan', 'No existe')
'No existe'

# Reasignacion y creacion de nuevos valores
>>> my_dict['Jaime'] = 20
>>> my_dict['Pedro'] = 25
>>> my_dict
{'David': 35, 'Erika': 32, 'Jaime': 20, 'Pedro': 25}
>>>

# Iterar sobre un diccionario
>>> for llaves in my_dict:
...     print(llaves)
... 
David
Erika
Jaime
Pedro
>>>  

# Iterar explicitamente en llaves
>>> for llaves in my_dict.keys():
...     print(llaves)
... 
David
Erika
Jaime
Pedro
>>>

# Iterar explicitamente en valores
>>> for valores in my_dict.values():
...     print(valores)
...
35
32
20
25

# Iterar explicitamente en llaves
>>> for llaves, valores in my_dict.items():
...     print(llaves, valores)
... 
David 35
Erika 32
Jaime 20
Pedro 25


>>> 'David' in my_dict
True
>>> 'Jose' in my_dict
False
>>>
```

## Pruebas y debugging

### 26 Pruebas de caja negra

Se conoce como caja negra porque suponemos no conocer laimplementacion

* Se basa en la especificacion de la funcion o el programa
* Prueba inputs y valida outputs
* Unit testing (funcion por funcion) o integration testing (todos los modulos funcionan entre si).

Test driven developtment: Antes de escribir una funcion vamos a escribir las pruebas de la  misma, podemos plantearnos todos los casos posibles.

```py
import unittest

def suma(num_1, num_2):
    return num_1 + num_2

class CajaNegratest(unittest.TestCase):

    def test_suma_dos_positivos(self):
        num_1 = 10
        num_2 = 5

        resultado = suma(num_1, num_2)

        self.assertEqual(resultado, 15)



    def test_suma_dos_negativos(self):
        num_1 = -10
        num_2 = -7

        resultado = suma(num_1, num_2)

        self.assertEqual(resultado, -17)

if __name__ == "__main__":
    unittest.main()
```

### 27 Pruebas de caja de cristal

* Se basan en el flujo del programa
* Prueba todos los caminos posibles de una funcion. Ramificacion, bucles for y while, recursion.
* Regression testing o mocks.

```py
import unittest

def es_mayor_de_edad(edad):
    if edad >= 18:
        return True
    else:
        return False


class CajaNegratest(unittest.TestCase):
    
    def test_es_mayor_de_edad(self):
        edad = 20

        resultado = es_mayor_de_edad(edad)

        self.assertEqual(resultado, True)
    
    def test_es_menor_de_edad(self):
        edad = 15

        resultado = es_mayor_de_edad(edad)

        self.assertEqual(resultado, False)

if __name__ == "__main__":
    unittest.main()
```

### 28 Debugging

Para reducir  bugs  hay que usar tests.

#### Reglas generales

* No te molestes con el debugguer. Aprende a utilizar el print statement.
* Estudia los datos disponibles
* Utilizalos datos para crear hipotesis y experimentos. Metodo cientifico
* Ten una mente abierta. Si entendieras el programa, probablemente no habrian bugs.
* Lleva un registro de lo que has tratado, preferentemente en la forma de tests.

#### Diseno de exprerimentos

* Debugear es u proceso de busqueda. Cada pruebea ebe acotar elespacio de busqueda.
* Busqueda binaria con print statements (divide y venceras).

#### Errores comunes

* Encuentra a los sospechosos comunes.
* En lugar de preguntarte porque un programa no funciona ,preguntatepor que esta funcionando de esta manera es posible que el blug no se encuentre donde crees que esta
* Explicale el problema a otra persona. De preferencia que no tenga contexto
* Lleva un registro de lo que has tratado, preferentemente en la forma de test.
* Vete a dormir.

## Excepciones y afirmaciones

### 29 Manejo de excepciones

Las excepciones ocurren cuando se presenta un error en nuestro codigo.

* Son muy comunes en la programacion. No tienen anda de excepcional.
* Las excepciones de Python normalmente se relacionan con errores de semantica.
* Se pueden crear excepciones propias.Cuando una excepcion no se maneja (unhandeled exception), el programa termina en error.

