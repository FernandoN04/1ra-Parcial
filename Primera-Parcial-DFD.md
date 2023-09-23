# PRIMERA PARCIAL
### <span style="color: red"> Diagrama 1: </span>
Obtener la edad promedio de N personas preguntando su año de nacimiento asumiendo que el año actual es 2023.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Comenzamos el diagrama e inicializamos las variables para crear un acumulador y un contador.

2. Preguntamos al usuario cuántas personas ingresarán para calcular el promedio de edades.
3. Guardamos la cantidad de personas en una variable llamada "Personas".
4. Establecemos una condición para asegurarnos de que el usuario ingrese un dato válido; en caso contrario, lo redirigimos para que vuelva a intentarlo.
5. Luego solicitamos al usuario que ingrese el año de nacimiento de la persona y lo almacenamos en una variable llamada "AN".
6. Creamos dos condiciones para validar que el dato ingresado en la variable "AN" sea válido; en caso contrario, lo rechazamos.
7. Incrementamos el contador y luego realizamos una operación para acumular las edades ingresadas.
8. Establecemos una última condición para verificar si el contador es igual a la cantidad de personas, lo que nos permitirá calcular el promedio; de lo contrario, volvemos a solicitar las edades restantes de las personas.
9. Finalmente, calculamos el promedio dividiendo el acumulador de edades por la cantidad de personas y presentamos el resultado. Luego cerramos el diagrama.

![DFD1](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/46718149-cf88-470b-8be8-e935279b5db2)

| c | s | Personas | Personas >= 2 | AN | AN >= 1900 | AN < 2023 | c = c + 1 | s = AN - 2023 | c >= Personas | prom = s / Personas |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ----------- | ----------- |
| 0 | 0 | 1 | 1 >= 2 NO | x | x  | x | x | x  | x  | x |
| 0  | 0  | 2 | 2 >= 2 SI | 2004 | 2004 >= 1900 SI  | AN < 2023 SI  | 0 = 0 + 1  | s = 2004 - 2023  | 1 >= 2 NO  | |
| 1  | 19  |   |   | 2010  | 2010 >= 1900 SI  | 2010 < 2023 SI  | 1 = 1 + 1  | s = 2010 - 2023  |  2 >= 2 SI | 0 = 32 / 2 |

### <span style="color: red"> Diagrama 2: </span>
Obtener el promedio de N numeros positivos.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, empezamos inicializando las variables de contador y acumulador.

2. Pedimos al usuario que ingrese la cantidad de numero a promediar y la almacenamos en la variable "i".
3. Realizamos una condicion para validar si la cantidad de numeros es mayor a 2, si no lo regresamos a volver a ingresar la cantidad.
4. Despues de validar le pedimos al usuario que ingrese el primer numero, lo almacenamos en la variable "n" la validamos para ver si cumple la condicion de mayor a 0 ya que no permitimos numeros negativos en el promedio.
5. Realizamos el proceso de ir almacenando cada numero ingresado en la variable "s" y aumentamos el contador.
6. Validamos si se cumple la condicion de la cantidad de numeros ingresado si aun no han pasado las veces que el usuario pidio seguimos el ciclo hasta terminar.
7. Para finalaizar sacamos el promedio dividiendo el total de numeros sumado y dividiendolo la cantidad de numeros ingresados, imprimimos el resultado y cerramos el diagrama.

![DFD2](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/4ce98a57-79a2-4a15-81cc-7d92c0154b88)

| c | s | i | i >= 2 | n | n > 0 | s = s + n | c = c + 1 | c >= i | prom = s / i |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ----------- | 
| 0 | 0 | 1 | 1 >= 2 NO | x | x  | x | x | x  | x |
| 0  | 0  | 2 | 2 >= 2 SI | 5 | 5 >= 0 SI  | 0 = 0 + 5  | 0 = 0 + 1  | 1 >= 2 NO ||
| 1  | 5  |  |  | 25  | 25 >= 0 SI  | 5 = 5 + 25  | 1 = 1 + 1  | 2 >= 2 SI  |  0 = 30 / 2 |

### <span style="color: red"> Diagrama 3: </span>
Obtener el promedio de 3 numeros cualquiera.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, inicializamos las variables una acumuladora y otra de conteo.

2. Pedimos al usuario un numero y lo almacenamos en la variable "n", despues lo validamos en una condicion que compare si ese dato ingresado es mayor a cero, si no es el caso lo regresamos dando un mensaje de corrección.
3. Despues la variable "n" la sumamos en el acumulador para los demas numeros que se ingresaran.
4. Aumentamos el contador y lo validamos en la condicion si ya ha sido ingresado los 3 numeros pasara al siguiente paso si no regresara a preguntar los numeros faltantes.
5. Para finalizar obtendremos el promedio dividiendo el acumulador por el contador o la cantidad de numeros ingresados en este caso 3, mostraremos el mensaje de cuanto fue el promedio y cerramos el diagrama.

![DFD33](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/d5159918-db0a-4ed9-a13e-474186745d9f)

| c | s | n | n > 0 | s = s + n | c = c + 1 | c >= 3 | prom = s / 3 | 
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| 0 | 0  | 0  | 0 > 0 NO  | X  | X  | X  | X  |
| 0 | 0  | 5  | 5 > 0 SI  | 0 = 0 + 5  | 0 = 0 + 1  | 1 >= 3 NO  |   |
| 1 | 5  | 7  | 7 > 0 SI  | 5 = 5 + 7 | 1 = 1 + 1  | 2 >= 3 NO |  |
| 2 | 12 | 3  | 3 > 0 SI  | 12 = 12 + 3  | 2 = 2 + 1  | 3 >= 3 SI  | 0 = 15 / 3  |


### <span style="color: red"> Diagrama 4: </span>
Elevar al cuadrado cualquier numero ingresado.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama pidiendole al usuario un numero para elevarlo al cuadrado.

2. Almacenamos el dato en la variable "n" y despues la validamos en la condicion si el numero es mayor o igual seguira el procedimiento si no cumple la condicion lo regresa imprimiendo un mensaje.
3. Realizamos la operacion multiplicando el numero por si mismo. 
4. Imprimimos el resultado y cerramos el diagrama.

![DFD4](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/b982b222-856b-4fbe-8167-ba1bf1388a5c)

| n | n >= 0 | cuadrado = n * n |
| ---------- | ---------- | ---------- |
| -1 | -1 >= 0 NO | X |
| 10 | 10 >= 0 SI  | 0 = 10 * 10 |

### <span style="color: red"> Diagrama 5: </span>
Capture N numeros enteros positivos obtenga la suma del cuadrado de los pares y el cubo de los impares.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama inicilizando variables un contador y dos acumuladores.

2. Preguntamos al usuario cuantos numeros ingresara y lo almacenamos en "i", lo validamos y es igual o mayor a 2 si no lo regresamos e imprimimos un mensaje.
3. Le pedimos un numero lo almacenamos en "n" lo validamos si es positivo proseguira el proceso si no lo regresaremos.
4. Aumentamos en contador y despues determinamos si un numero es par o impar, si da verdadero se hara un proceso para sacar la potencia al cuadrado del numero y guardarlo en el acumulador, si no es el caso y da falso pasara al otro proceso pero ahora al cubo.
5. Despues pasa por un condicionador para determinar si ya fueron ingresados todos los numeros si no es asi lo regresara para terminar de ingresar los numero faltantes, ya que de verdadero la condicion imprimira el resultado y cerramos el diagrama.

![DFD5](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/915ba60e-53ab-4ab9-be0b-88451248edad)

| c | i | cb | cd | i >= 2 | n | n >= 0 | c = c + 1 | n % 2 = 0 | cd = (cd) + (n * n) | cb = (cb) + (n * n * n) | c >= i |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ----------- | ---------- | ----------- |
| 0  | 1  | 0  | 0 | 1 >= 2 NO  | x  | x | x | x  | x  | x |x  |
| 0 | 2 | 0 | 0  | 2 | 2 >= 2 SI  | 5 | 0 = 0 + 1 | 5 % 2 = 0 NO  | X  | 0 = (0) + (5 * 5 * 5) | 1 >= 2 NO  |
| 1 |   | 125  | 0 |   | 2  | 2 >= 0 SI  | 1 = 1 + 1  | 2 % 2 = 0 SI  | 0 = (0) + (2 * 2)  |   | 2 >= 2 SI  |


### <span style="color: red"> Diagrama 6: </span>
Obtener la suma de todos los cuadrados de N numeros capturados del teclado.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama inicializando las variables un contador y un acumulador.

2. Preguntamos al usuario cuantos numeros quiere usar y los almacenamos en "i", despues lo validamos si es igual o mayor a 2 si da falso tendremos que regresarlo e imprimirle un mensaje.
3. Despues de que la condicion fuera verdadera le pedimos al usuario ingresar un numero que almacenaremos en "n" y lo validaremos para analizar si es positivo.
4. Aumentamos el contador y realizamos la operacion al cuadradro del numero alamacenando en "s".
5. Hacemos otra condicion para comprobar si ya ha sido ingresado todos los numero si no es asi empezara el ciclo hasta que se cumpla la condicion.
6. Para finalizar la condicion da verdadero y le mostraremos al usuario el resultado, terminando cerramos el diagrama.

![DFD6](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/dc905af7-8a5d-4eae-a2eb-9db8874f12d3)

| c | s | i | i >= 2 | n | n => 0 | c = c + 1 | s = (s) + (n * n) | c >= i |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| 0  | 0  | 1  | 1 >= 2 NO | X | X | X  |X  | X  |
| 0  | 0  | 2  | 2 >= 2 SI | 5  | 5 >= 0 SI  | 0 = 0 + 1  | 0 = (0) + (5 * 5) | 1 >= 2 NO  |
| 1  | 125  |   | | 1  | 1 >= 0 SI | 1 = 1 + 1  | 125 = (125) + (1 * 1) | 2 >= 2 SI  |

### <span style="color: red"> Diagrama 7: </span>
Escriba un DFD que dado el año de nacimiento indique cuantos años va cumplir el siguiente año.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos diagrama preguntando el año de nacimiento, lo almacenamos en "AN".

2. Validamos si es mayor a 0 y menor a 2023 si no lo regresamos.
3. Para finalizar hacemos la operacion restando el año actual al de nacimiento y sumando un 1, terminamos imprimiendo el resultado cerrando el diagrama.


![DFD7](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/bd434245-5f79-4a53-a3ea-ec1593f47cd9)

| AN | AN >= 0 AND AN < 2023| CM = AN - 2023 + 1 |
| ---------- | ---------- | ---------- |
| 2024  | 2024 >= 0 AND 2024 < 2023 SI, NO  | X  |
| 2004  | 2004 >= 0 AND 2004 < 2023 SI, SI | 0 = 2004 - 2023 + 1  |



### <span style="color: red"> Diagrama 8: </span>
Obtenga la suma de 5 numeros capturados entre 5 y 10 inclusivo.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama inicializando variables el contador y acumulador, preguntamos cuantos numeros ingresar el usuario y lo almacenaremos en "i", lo validamos si "i" es mayor o igual a 2.

2. Le pedimos al usuario ingresar un numero lo validamos en una condicion con el intervalo de [5,10] y despues de dar verdadero aumentamos el contador.
3. Hacemos la operacion usando el acumulador para sumar los numeros y guardarlo.
4. Para finalizar validamos si ya se ingresaron todos los numeros luego de dar verdadero damo el resultado de la suma y cerramos el diagrama.

![DFD8](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/a8d8d39b-18e5-4207-993a-ec6d76c3d88f)

| c | s | i | i >= 2 | num | num >= 5 AND num <= 10 | c = c + 1 | s = s + num | c >= i |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| 0  | 0  | 1  | 1 >= 2 NO | X  | X  | X  | X  | X  |
| 0  | 0  | 2  | 2 >= 2 SI  | 6  | 6 >= 5 AND 6 <= 10 SI, SI | 0 = 0 + 1 | 0 = 0 + 6  | 1 >= 2 NO  |
| 1  | 6 |   |   | 5 | 5 >= 5 AND 5 <= 10 SI, SI  | 1 = 1 + 1  | 6 = 6 + 5  | 2 >= 2 SI  |

### <span style="color: red"> Diagrama 9: </span>
Una empresa desea calcular el sueldo total de varias personas bajo los siguintes rublos: presepciones, sueldo base, canasta basica, prima de antiguedad y deducciones, si el salario base exede los 10 mil pesos el ISR es el 30% y menos de eso el 20% de impuesto. Indique cuanto es el total de la nomina a pagar y cuantos son los impuestos que tiene que pagar el patron al SAT.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, inicializamos variables acumulativas y contadoras.

2. Pedimos al usuario la cantidad de empleados con la condicion de que al menos se 1.
3. Usamos el condicional para saber si ya han sido registrados los datos del empleado que en el momento apenas va empezando y dara falso.
4. Le pediremos los datos a resgitrar las persepciones y el sueldo base que se sumaran, despues aplicamos la canasta y la prima.
5. Ahora aplicamos el ISR pero antes hacemos la condicion si excede de 10,000 aplicaremos el 30%, si no el 20% se lo restamos al sueldo base.
6. Aumentamos el contador y guardamos el sueldo total y el impuesto.
7. Pasamos por la primera condicional dando verdadero ahora imprimira la nomina y los impuesto a pagar.
8. Cerramos el diagrama.

![DFD9](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/573bcea3-c654-43b2-97d2-65c7ebb024f5)

| p | p >= 1 | c >= p | pers | sb | cb = sb * 1.05 + pers | pa = sb * 1.03 | sba = pa + cb | sba >= 10000 | sbi = sb * 0.30 |sbi = sb * 0.20 |sbf = sba - sbi |sbbf = sbf + sba + sbbf |c = c + 1 |sat = sat + sbi |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- | ----------- |
| 1 | 1 >= 1 SI | 0 >= 1 NO | 10  | 50  | 0 = 50 * 1.05 + 10  | 0 = 52.5 * 1.03 | 0 = 52.07 + 2.57  | 54.07 >= 10000 NO  ||  0 = 54.07 * 0.20  | 0 = 54.07 - 10.81 |  0 = 43.25 + 0 |0 = 0 + 1  | sat = sat + 10.81 |


### <span style="color: red"> Diagrama 10: </span>
Genere la siguiente secuencia 0,1,0,1,0,1,0,1,0,1,0,1...0,1.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, imprimimos los mensajes 0 y 1 infinitamente ya que no pide detenerlo.

![DFD10](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/602b089e-bacf-4f96-a69e-ee4aee5180b2)

### <span style="color: red"> Diagrama 11: </span>
Preguntar un numero y determinar el dia de la semana que es.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, le pedimos al usuario un numero.

2. Depende del numero le dara el dia al usuario.
3. Si no es el caso y sobre pasa el numero de 1 a 7 le dara un error.
4. Cerramos diagrama.

![DFD11](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/bda1fa19-7bf2-49a6-aea7-db311234c389)

| n | 1 | 2 | 3 | 4 | 5 | 6 | 7 | Else |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| 10  | x  | x  | x  | x  | x | x  | x  | "Error"  |
| 5  | x  | x  | x  | x  | "Viernes"  | x  | x  | x  |


### <span style="color: red"> Diagrama 12: </span>
La tienda "Bronkos" debe vender productos a N alumnos, ofrecen: tortas, tacos, hot dogs y pizzas. Imprime el total que vendio cada producto y el total en general.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, inicializamos las variables contadoras.

2. Pedimos al usuario cuantos alumnos compraran y lo validamos debe al menos tener un alumnos para dar verdadero en la condicion.
3. Hacemos otra condicion que se usara despues que validara si ya pasaron todos los alumnos a comprar.
4. Abrimos un switch con 5 opciones las 4 del menu y una de error, tendra que elegir el usuario que opcion seleccionar y esta contara la opcion seleccionada ademas del contador global, si da error no la contara.
5. Para finalizar pasamos por la condicion del anterior paso cuando sea verdadero imprimira el resultado y cerraremos el diagrama.

![DFD12](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/0fda0789-cd84-44be-8e7c-34cbb883f8b5)

| c | ta | to | pi | hd | n | n >= 1 | c >= n | a | ta = ta + 1 | to = to + 1 | pi = pi + 1 | hd = hd + 1 | Else| c = c + 1|
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ----------- | ---------- | ---------- | ---------- | ----------- | ----------- |
| 0  | 0  | 0  | 0  | 0 | 0  | 0 >= 1 NO | X | X | X | X | X | X | X |X|
| 0  | 0  | 0  | 0  | 0  | 1  | 1 >= 1 SI  | 0 >= 1 NO  | 2  | X | 0 = 0 + 1| X | X | X | 0 = 0 + 1|
| 1  | 0  | 1  | 0  | 0  |  |  | 1 >= 1 SI  |   |  | | |  |  | |

### <span style="color: red"> Diagrama 13: </span>
Crea una calculadora funcional que sume, reste, divide y multiplique dos numeros.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, preguntamos al usuario que elija un numero.

2. Pedimos otro numero y abrimos un menu despues usamos un switch.
3. En el switch abrimos 5 opciones suma, resta, division, multiplicacion y un error.
4. Ya dependera la opcion que elija el usuario y imprimira el resultado.
5. Cerramos diagrama.

![DFD13](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/4eb166e4-f310-4270-aa93-9ae1175ed63c)

| n1 | n2 | o | r = n1 + n2 | r = n1 - n2 | r = n1 / n2 | r = n1 * n2 | Else |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| 5  | 5  | 5  | x  | x  | x  | 0 = 5 * 5  | x |


### <span style="color: red"> Diagrama 14: </span>
Pedir al usuario un numero para reproducir una serie de 1 y 0.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, inicializamos variables un contador y una bandera con el valor de 0.

2. Preguntamos al usuario cuantas veces quiere reproducir la secuencia.
3. Validamos que ya paso la secuencia las veces pedidas por el ususario.
4. Creamos un condicional que compara si la bandera es igual a 0, si es asi imprimira la bandera con el valor cero, despues la bandera cambia su valor a 1 y aumneta el contador y pasa por la condicion anterior.
5. Despues de pasar vuelve a comparar la bandera si es igual a 0 esta vez no sera verdadero y pasara a imprimir el valor de 1, cambiara la bandera de nuevo y asi las veces que lo pidio el usuario.
6. Cerramos el diagrama.

![DFD14](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/f978f5cd-56c9-4921-952f-01b0b29b46f9)

| c | b | i| c >= i | b == 0 | b = 1 | b = 0 | c = c + 1|
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| 0  | 0 | 2  | 0 >= 2 NO  | 0 == 0 SI  | 0 = 1 |   | 0 = 0 + 1  |
| 1 | 1  |   | 1 >= 2 NO  | 1 == 0 NO  |   | 1 = 0 | 1 = 1 + 1  |
| 2 | 0  |   | 2 >= 2 SI  |   |   |  |  |


### <span style="color: red"> Diagrama 15: </span>
Obtenga el cubo de un numero.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, imprimimos que ingrese un numero el usuario y lo validamos si es positivo.

2. Para terminar realizamos la operacion del numero al cubo y cerramos el diagrama mostrando la respuesta.

![DFD155](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/acb5e911-7a4b-4d40-90cd-852f27c5feee)

| n | n >= 0 | c =  n * n * n |
| ---------- | ---------- | ---------- |
| 3  | 3 >= 0 SI  | 0 = 3 * 3 * 3  |


### <span style="color: red"> Diagrama 16: </span>
Obtenga la edad de una persona.

#### <span style="color: green"> ANÁLISIS: </span> 

1. Iniciamos el diagrama, preguntando al usuario el año de nacimiento.

2. Validamos que no pase de 2023 o sea antes de 0.
3. Despues restamos el año actual con el de nacimiento.
4. Imprimimos el resultado y cerramos el diagrama.

![DFD166](https://github.com/FernandoN04/1ra-Parcial/assets/145720700/ab001b4d-1d49-4f17-b615-74dfd01a8168)

| an | an > 0 AND an < 2023| edad = an - 2023|
| ---------- | ---------- | ---------- |
| 2004 | 2004 > 0 AND 2004 < 2023 SI, SI | 0 = 2004 - 2023  |
