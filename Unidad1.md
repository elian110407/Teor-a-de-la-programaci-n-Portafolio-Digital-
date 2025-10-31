# ⚛️ Unidad 1: Algoritmos y Programación Básica 💻
---
## 💻 Contenidos de la Unidad
### Algoritmos, Pseudocódigo, Diagrama de Flujo ✨

* 💿 **Algoritmos**

    Un **algoritmo** es una serie de secuencias organizadas de manera lógica y limitada que resuelven un problema específico. Los algoritmos se clasifican en dos:
    * **Algoritmos Cualitativos:**
        Implican la descripción a través de frases y palabras[1].
    * **Algoritmos Cuantitativos:**
        Se refieren al uso de cálculos o fórmulas matemáticas[1].

* 💾 **Pseudocódigos**

    El **pseudocódigo** es una forma de describir un algoritmo o programa de computadora utilizando una mezcla de lenguaje natural, como el español. Su objetivo es permitir a los programadores centrarse en la lógica del algoritmo sin preocuparse por las reglas de un lenguaje de programación específico, sirviendo como un borrador o esquema legible antes de la codificación final.\[2]

    * 👨‍💻 **Ejemplos:**

    En este ejercicio utilizaremos el pseudocódigo para crear un código que nos permita calcular cuánto debería cobrar un pintor por el metro cuadrado de pintura.

    * **Ejemplo 1: Cobrar pintura por metro cuadrado.**
        ```
        Algoritmo Cobrar_pintura
        	Definir metroscuadro, precio, presupuesto Como Real
        	// Datos de entrada //
        	Escribir 'Ingrese la cantidad de metros cuadrados:'
        	Leer metroscuadro
        	Escribir 'Ingrese el precio por el metro cuadrado:'
        	Leer precio
        	// Proceso //
        	presupuesto <- (metroscuadro * precio)
        	// Datos de salida //
        	Escribir 'El presupuesto por los metros cuadrados de pintura es de:', presupuesto
        FinAlgoritmo
        ```

---

### *Explicación del Código:* 📝

* Lo primero que tenemos que hacer es **identificar las variables**; en este caso, las definiremos como **reales**.
* Utilizamos los `"//"` para poder incluir **comentarios** dentro del código, pero estos comentarios no afectan en nada la ejecución.
* Después de esto, utilizamos la función **"Escribir"** para que el usuario sepa qué datos debe ingresar en ese apartado.
* Como siguiente paso, utilizaremos la función **"Leer"** y luego la variable a la cual será asignado el dato que el usuario ingresará.
* Después de definir las variables, continuamos con el **cálculo**. Escribimos la variable, después un **`<-`** (o a veces se usa `=`), lo que significa que lo escrito después será el valor que se le asignará a la variable.
* Después de escribir la fórmula, volveremos a usar la función **"Escribir"** para poder mostrar al usuario el resultado final, separando con una coma y luego la variable, con lo cual se le mostrará al usuario el resultado de la operación.

---

### *Pruebas de Escritorio* 📊

| N° | Metros Cuadrados | Precio por Metro Cuadrado | Operación | Resultado |
| :--- | :---: | :---: | :---: | ---: |
| 1 | 8 | $15 | `presupuesto = 8 * 15` | $120 |
| 2 | 20 | $30 | `presupuesto = 20 * 30` | $600 |
| 3 | 4 | $20 | `presupuesto = 4 * 20` | $80 |

---

* 📊 **Diagramas de Flujo**

    Un **Diagrama de Flujo** es una representación gráfica y secuencial de un algoritmo o proceso, utilizando un conjunto estandarizado de símbolos geométricos para ilustrar las operaciones, el flujo de datos y los puntos de decisión desde el inicio hasta el final.\[3]

    * 📁 **Ejemplos:**

    

<p align="center">
  <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgFnZ4ClrAACm1Kke4AslbbEi2w-iYNcDJgIEHfcMXGaoFsq7Frj5KMgjpl1sDeb1DBM9aCdHxicgoZWfrf1tFGdHZ9mo3wnNo7wi4c8C5RHTbIrH2pBm2h4s2kan93fESgl7mT5ZVs-rPAnp4AAdXirUFe7rqYi2RDSqD1Vw2v6P-hykyDwW5MZ50AdEkg/w645-h405/Captura%20de%20pantalla%202025-10-25%20133423.png" alt="Descripción" width="75%">
</p>


---

### *Explicación del Diagrama de Flujo* 🔍

* Muestra la estructura del algoritmo de una manera **visual**.
* Los rectángulos punteados de verde representan las **instrucciones**.
* La figura del rectángulo rojo representa la función **"Leer"** (entrada de datos).
* La figura del rectángulo amarillo representa la **operación** (proceso).
* Las **flechas** demuestran el flujo de la secuencia que sigue el algoritmo.

---

### 🚶‍➡️🏆 Programación por Bloques 🧱

La **Programación por Bloques** es un método de programación visual que permite a los usuarios crear programas al arrastrar, soltar y encajar bloques gráficos que representan comandos o estructuras de programación. Está diseñado para ser intuitivo y accesible, especialmente para principiantes y niños, ya que elimina la necesidad de escribir código textual y evita los errores de sintaxis que son comunes en la programación tradicional.\[4]

* 📁 **Ejemplos:**

<p align="center">
  <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgVZclfKlb_xw_DIDytYFOiNDR6jJvCHmf3k3fWCerWWGfdTvXZchwhXhtsHbyXH8oKLuyVEdJIc9dByY7vpXCtVhu0XDlorTboz1vuRbGsvJvh90EDluJilGIxKo7FbXd0opTnbkuwFKfirTnYzjAqGFfbih9goqtwhuC2aJ8Rf3cyWOE8RCCXT3u0Zy5t/s1080/Captura%20de%20pantalla%202025-10-25%20134314.png" alt="Descripción" width="75%">
</p>

---

### *Explicación Práctica de la Programación por Bloques* 💡

En esta imagen se muestra una estructura simple de un algoritmo construido por bloques, y se muestran dos bloques:

* El primer bloque da una orden en **bucle** que se repite hasta llegar a un cierto punto.
* El segundo bloque da la orden de **avanzar hacia adelante** una sola vez.

La forma en que están apilados los bloques indica el **orden** en el que se ejecutará la acción hasta llegar a su punto indicado.

---

### 🖥️ ⚙️ Ejemplos de Algoritmos con Estructuras Lineales/Secuenciales ➡️

Para esta parte, elegí un algoritmo que me permita calcular el **precio final de un producto con descuento**, y luego lo realizaré en pseudocódigo y en el lenguaje de programación **C**.

* 🔍 **Actividad en Pseudocódigo**
    ```
    Algoritmo CalcularPrecioConDescuento

    	Definir precio_original, porcentaje_descuento, precio_final Como Real;
    	Definir descuento Como Real;
    	// Datos de entrada //
    	Escribir "Ingresa el precio original del producto:"
    	Leer precio_original;
    	Escribir "Ingresa el porcentaje de descuento:"
    	Leer porcentaje_descuento;
    	// Proceso //
    	descuento = precio_original * porcentaje_descuento / 100;
    	precio_final = precio_original - descuento;
    	// Datos de salida //
    	Escribir "El descuento aplicado es de: $", descuento;
    	Escribir "El precio final con el descuento es de: $", precio_final;
    FinAlgoritmo
    ```

---

En este algoritmo, se le pide al usuario que ingrese el **valor del precio original** y el **porcentaje de descuento**. Después, escribimos la **fórmula** para calcular el descuento y el precio final. A continuación, procedemos a mostrar el **mensaje final** donde se mostrará el resultado del descuento aplicado y el precio final.

---

* 💽 **Actividad en C**
    ```c
    #include <stdio.h>
    #include <math.h>

    int main() {
    
    float precio_original;
    float porcentaje_Descuento;
    float precio_Final;
    float descuento;
    
    /* Datos de entrada */
    
    printf("Ingrese el precio original:\n");
    scanf("%f", &precio_original);
    
    printf("Ingrese el porcentaje de descuento:\n");
    scanf("%f", &porcentaje_Descuento);
    
    /* Proceso */
    
    descuento = precio_original * porcentaje_Descuento / 100;
    precio_Final = precio_original - descuento;
    
    /* Datos de Salida */
    
    printf("El descuento aplicado es de: %f\n", descuento);
    printf("El precio final con el descuento es de: %f\n", precio_Final);
    
    return 0;
    }
    ```

---

### *Explicación del Algoritmo en C* ⚙️

* Primero, debemos incluir la biblioteca `"#include <stdio.h>"` porque esta permite usar las funciones `"printf"` y `"scanf"`, que son necesarias para la entrada y salida de datos. También incluimos la biblioteca `"<math.h>"` ya que esta nos permite resolver fórmulas matemáticas (aunque para este ejemplo no es estrictamente necesaria, su inclusión es correcta si se planean más cálculos).
* A continuación, escribimos `"int main() {"`, que es el iniciador del programa, ya que **`main`** es el nombre de la función de C que permite el inicio y ejecución de todo lo que escribimos dentro de las llaves. Siempre al final de cada instrucción pondremos **`;`** (punto y coma), lo que indica el fin de la instrucción.
* En C hay un ligero cambio con respecto al pseudocódigo, ya que aquí primero pondremos el **tipo de variable** y luego el nombre. En este caso, se utiliza la variable `"float"` porque permite leer números decimales.
* Ahora, escribiremos los datos de entrada, usando `"printf()"` (similar a "Escribir") y `"scanf()"` (similar a "Leer"). En el `printf`, usamos `"\n"` para que la función `scanf` se muestre debajo del texto. En la función `scanf`, usamos la **máscara de formato** `"%f"` para indicar que el programa espera un valor de tipo **`float`**. Después de esto, se pone una coma e irá el símbolo **`&`** (ampersand), que le dice al programa que guarde el valor ingresado por el usuario dentro de la variable definida.
* Después, escribiremos la **fórmula** para resolver el ejercicio, que no cambia con respecto al pseudocódigo.
* Finalmente, escribimos los datos de salida usando `printf`. Luego de escribir el mensaje final, se pone la máscara `"%f"`, que es como si diera un espacio exclusivo para el resultado. Después, ponemos una coma y la variable.
* Al último, ponemos `"return 0;"`, que le dice al programa que la función `main` terminó exitosamente, y cerramos el código con **`}`**.

---

### Pruebas de Escritorio 📋

| N° | Precio Original | Porcentaje de Descuento | Proceso | Descuento | Precio Final |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | $120 | 35% | `descuento = 120 * 35 / 100` | $42 | $78 |
| 2 | $1250 | 75% | `descuento = 1250 * 75 / 100` | $937.5 | $312.5 |
| 3 | $500 | 67% | `descuento = 500 * 67 / 100` | $335 | $165 |

---
### ❓🤷‍♂️ Principales Dificultades en la Aplicación de los Contenidos 🛑

* El principal problema que tuve al realizar códigos en lenguaje de programación fue que muchas veces **no compilaba el código** por algún error en la escritura.
* También, el **aprender el lenguaje de C**, ya que en PSeInt utilizábamos palabras en español y en C se utiliza un lenguaje diferente para escribir cada instrucción del código.
* El **olvido del punto y coma** (`;`), que es el cierre de instrucción más común en C y cuya ausencia genera errores de sintaxis.
* Otra dificultad fue **aprender qué librerías** se deben utilizar para los distintos códigos.

---
### 🕵️ 🎓 Reflexión Crítica de los Aprendizajes de la Unidad. 🤔

En la Unidad aprendí muchas cosas sobre cómo crear un código en lenguaje de programación y cuál es su estructura. También aprendí que, para empezar en el mundo de la programación, tenemos una herramienta que nos facilita la entrada a este mundo: los **pseudocódigos**. Son fáciles de utilizar, ya que usamos el idioma español para poder realizar los códigos. Cuando ya sepamos las bases de las estructuras de los lenguajes de programación, podemos pasar a alguno más avanzado, pero lo más importante es no tener como prioridad un solo lenguaje, porque en la vida laboral necesitaremos **dominar varios lenguajes de programación**.

---

<p align="right">
  <a href="index.md">Volver a la página principal</a>
</p>
