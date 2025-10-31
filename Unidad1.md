# ⚛️ Unidad 1
##  💻Contenidos de la Unidad
### Algoritmos,pseudocodigo,diagrama de flujo.
* 💿 Algoritmos

  Un algoritmo es una serie de secuencias organizadas de manera lógica y limitada que resuelven un problema específico,los algoritmos se clasifican en dos:
  * Algoritmos Cualitativos:
  
    Implique la descripción a través de frases y palabras.[1]
    
  * Algoritmos Cuantitativos:
  
    Se refiere al uso de cálculos o fórmulas matemáticas.[1]
    
* 💾 Pseudocodigos

  El pseudocódigo es una forma de describir un algoritmo o programa de computadora utilizando una mezcla de lenguaje natural como el español, su objetivo es  permitir a los programadores centrarse en la lógica del algoritmo sin preocuparse por las reglas de un lenguaje de programación específico, sirviendo como un borrador o esquema legible antes de la codificación final.[2]
  
  * 👨‍💻 Ejemplos:

 En este ejercicio utilizaremos el pseudocodigo para crear un codigo que nos permita calcular cuanto deberia de cobrar un pintor por el metro cuadrado de pintura.

* Ejemplo 1: Cobrar pintura por metro cuadrado.
 ```
Algoritmo Cobrar_pintura
	Definir metroscuadro, precio, presupuesto Como Real
	// Datos de entrada//
	Escribir 'Ingrese la cantidad del metro cuadrado:'
	Leer metroscuadro
	Escribir 'ingrese el precio por el metro cuadrado:'
	Leer precio
	// Proceso//
	presupuesto <- (metroscuadro*precio)
	// Datos de salida//
	Escribir 'El presupuesto por los metros cuadrados de pintura es de:', presupuesto
FinAlgoritmo
```
---

### *Explicación del código:*

* Lo primero que tenemos que hacer es identificar las variables, en este caso las definiremos como reales.
* Utilizamos los "//" para poder comentarios dentro del codigo pero estos comentarios no afectan en nada en la ejecucion.
* Despues de esto utilizamos la funcion "Escribir" para que el usuario vea que datos debe de ingresar en ese apartado.
* Como siguiente paso utilizaremos la funcion "Leer" y luego la variable a la cual será asignada el dato que el usuario ingresara.
* Despues de definir las variables continuamos con el cálculo, escribimos la variable, despues de eso un "=" lo que significa que lo escrito despues del igual sera el valor que sera entregada a la variable.
* Despues de escribir la formula, volveremos a usar la funcion "Escribir" para poder mostrar al usuario el resultado final separando con una coma y luego la variable, la cual se le mostrara al usuario el resultado de la operacion.
  
---

### *Pruebas de Escritorio*

<p style="text-align:center; font-size:12px;">Tabla 1. Prueba de escritorio

| N° | Metro cuadrado | Precio por metro cuadrado | Operación | Resultado |
| :--- | :---: | :---: | :---: | ---: |
| 1    | 8  | $15  | presupuesto= 8 * 15 | $120 |
| 2    | 20  | $30  |  presupuesto= 20 * 30 | $600 |
| 3    | 4   | $20   |  presupuesto= 4 * 20 | $80 |

---

* 📊 Diagramas de flujo

  Un Diagrama de Flujo es una representación gráfica y secuencial de un algoritmo o proceso, utilizando un conjunto estandarizado de símbolos geométricos para ilustrar las operaciones, el flujo de datos y los puntos de decisión desde el inicio hasta el final.[3]

  * 📁Ejemplos:
 
<p align="center">
  <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgFnZ4ClrAACm1Kke4AslbbEi2w-iYNcDJgIEHfcMXGaoFsq7Frj5KMgjpl1sDeb1DBM9aCdHxicgoZWfrf1tFGdHZ9mo3wnNo7wi4c8C5RHTbIrH2pBm2h4s2kan93fESgl7mT5ZVs-rPAnp4AAdXirUFe7rqYi2RDSqD1Vw2v6P-hykyDwW5MZ50AdEkg/w645-h405/Captura%20de%20pantalla%202025-10-25%20133423.png" alt="Descripción" width="75%">
</p>

 ---

 ###  *Explicación del diagrama de Flujo* 

* Muestra la estructura del algoritmo de una manera visual.

* Los rectangulos punteadas de verde representan  las instrucciones.

* La figura del rectángulo rojo representa la función "leer".

* Las figura del rectangulo amarillo representa la operacion.

* Las flechas demuestran el flujo de la secuencia que sigue el algoritmo.

 ---
 
### 🚶‍➡️🏆Programación por bloques

La Programación por Bloques es un método de programación visual que permite a los usuarios crear programas al arrastrar, soltar y encajar bloques gráficos que representan comandos o estructuras de programación.Está diseñado para ser intuitivo y accesible, especialmente para principiantes y niños, ya que elimina la necesidad de escribir código textual y evita los errores de sintaxis que son comunes en la programación tradicional. [4]

  * 📁Ejemplos:

<p align="center">
  <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgVZclfKlb_xw_DIDytYFOiNDR6jJvCHmf3k3fWCerWWGfdTvXZchwhXhtsHbyXH8oKLuyVEdJIc9dByY7vpXCtVhu0XDlorTboz1vuRbGsvJvh90EDluJilGIxKo7FbXd0opTnbkuwFKfirTnYzjAqGFfbih9goqtwhuC2aJ8Rf3cyWOE8RCCXT3u0Zy5t/s1080/Captura%20de%20pantalla%202025-10-25%20134314.png" alt="Descripción" width="75%">
</p>

---

###  *Explicación práctica de la programación por bloques*
En esta imagen se muestra una estructura simple de un algoritmo construido por bloques y se muestran dos bloques:

* El primer bloque da una orden en bucle que se repite hasta llegar a un cierto punto.
* El segundo bloque da la orden de avanzar hacia adelante una sola vez.

La forma en que estan apilados los bloques dice el orden en el que se ejecutara la accion hasta llegar a su punto indicado.

---

###  🖥️ ⚙️ Ejemplos de algoritmos con estructuras lineales/secuenciales

Para esta parte elegi un algoritmo que me permita Calcular cuanto sera el precio final de un producto con descuento, y otro codigo que me permita ver el promedio de nota para el colegio en Pseint y luego lo realizare en lenguaje de programacion C.

* 🔍 Actividad en Pseudocodigo
```
Algoritmo CalcularPrecioConDescuento

	Definir precio_original, porcentaje_descuento, precio_final Como Real;
	Definir descuento Como Real;
	//Datos de entrada//
	Escribir "Ingresa precio original del producto:"
	Leer precio_original;
	Escribir "Ingresa el porcetaje de descuento:"
	Leer porcentaje_descuento;
	//Proceso//
	descuento =  precio_original * porcentaje_descuento/100;
	precio_final = precio_original - descuento;
	//Datos de salida//
	Escribir "El descuento aplicado es de: $", descuento;
	Escribir "El precio final con el descuento es de: $", precio_final;
FinAlgoritmo
```

---

En este algoritmo se le muestra al usuario que ingrese el valor del precio original, y el porcentaje del descuento, despues escribimos la fórmula para sacar el descuento y el precio final, a continuacion despues de escribir la  fórmula procedemos a escribir el mensaje final donde se mostrará el resultado de la aplicacion del descuento y su precio final con el descuento aplicado.

---

* 💽 Actividad en C
```
#include <stdio.h>
#include <math.h>

int main () {;

float precio_original;
float porcentaje_Descuento;
float precio_Final;
float descuento;

/*Datos de entrada*/

printf("Ingrese precio:\n");
scanf("%f", &precio_original);

printf("Ingresa el porcentaje de descuento:\n");
scanf("%f", &porcentaje_Descuento);

/*Proceso*/

descuento = precio_original * porcentaje_Descuento/100;
precio_Final = precio_original-descuento;

/*Datos de Salida*/

printf("El descuento aplicado es de: %f\n",descuento);
printf("El precio final con el descuento es de: %f\n", precio_Final);

}

```

---

### *Explicacion del algoritmo en C*
* Primero debemos incluir la biblioteca "<stdio.h>" por que esta permite incluir las funciones "printf" y "scanf" que son necesarias para escribir los datos de entrada y salida, tambien incluimos la biblioteca <math.h> ya que esta nos permite resolver formulas matematicas.
* A continuacion escribimos "int main() {" que es el iniciador del programa, ya que "main" es el nombre de la función de C que nos permite dar el inicio y ejecución de todo lo que escribimos dentro de las llaves, simpre al ultimo de cada linea pondremos ";" esto quiere decir que hasta ahi es la intruccion.
* En C hay un ligero cambio del pseudocodigo, ya que aqui primero pondremos que tipo de variable será y luego el nombre de la variable, en este caso se utilizara la variable "float" ya que nos permite leer decimales pero en pequeñas cantidades.
* Ahora escribiremos los datos de entrada, en donde se usaremos "printf()" que es lo mismo que "Escribir" y "scanf()" que es " Leer". En el printf se usamos "\n" para que la función scanf se muestre debajo del texto, en esta función se usamos la máscara "%f" para decir que el programa espera un valor de tipo "float", depues de esto se pone una coma e ira el simbolo "&" que le dice al programa que guarde el valor ingresado por el usuario dentro de la varibale definida.
* Despues escribiremos la formula para resolver el ejercicio que no cambia en nada en cuanto lo que hacemos en pseudocodigo.
* Escribimos los datos de salida, usando printf, luego de escribir el mensaje final se pone la máscara "%f" que es como si diera un espacio exclusivo para el resultado, despues ponemos una coma y la variable.
* Al ultimo ponemos "return 0;", que le dice el programa que el main termino, y cerramos en condigo con "}".

---

### Pruebas de escritorio.
<p style="text-align:center; font-size:12px;">Tabla II. Prueba de escritorio

| N°1 |precio original |porcentaje del descuento | Proceso | Resultado |
| :--- | :--- | :--- | :--- | :--- |
| 1 | $120 | 35% |descuento =  120 * 35/100 | $42 |
| 2 | $1250 | 75% |descuento =  1250 * 75/100 | $937.5 |
| 3 | $500 | 67% |descuento =  500 * 67/100 | $335 |

### ❓🤷‍♂️ Principales dificultades en la aplicación de los contenidos

* Los Princiaples problemas que tuve al realizar codigos en lenguaje de programacion esque muchas veces no copilaba en codigo por algun error en la escritura del codigo.
* Tambien el aprenderme el lenguaje de C ya que en pseint utilizabamos palabras en español y en C se utiliza diferente lenguaje para para escribir cada instruccion del codigo.
* Olvido del Punto y Coma, es el cierre de instrucción más común en C y su ausencia genera errores de sintaxis. Otra dificultad fue aprenderme que librerias nomas se deben utilizar para los distintos codigos.
---
### 🕵️ 🎓 Reflexión crítica de los aprendizajes de la unidad.

En la Unidad aprendi muchas cosas sobre como crear un codigo en lenguaje de programacion y cual es su estructura, tambien aprendi que para empezar en el mundo de la programacion tenemos una herramiento la cual nos facilita la entrada a este mundo y esa herramienta son los pseudocodigos porque es facil de utilizar ya que utlizamos el idioma español para poder realizar los codigos, cuando ya sepamos las bases de las estructuras de los lenguajes de programacion podemos pasar a alguno otro más avanzado pero lo mas importante es no tener como prioridad un solo lenguaje porque en la vida laboral necesitaremos dominar algunos lenguajes de programación.

<p align="right">
  <a href="index.md">Volver a la página principal</a>
</p>
