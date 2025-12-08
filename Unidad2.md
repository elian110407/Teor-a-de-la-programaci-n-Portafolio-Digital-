# ⚛️ CONTENIDO UNIDAD 2

---

### 🖥️🏆*ESTRUCTURAS CONDICIONALES*

---

### 📄💾*ESTRUCTURA CONDICIONAL SIMPLE (IF)*

La estructura condicional simple (IF) es una herramienta de programación que permite ejecutar un bloque de código solo si una condición específica es verdadera.

* Si la condición dentro del if se cumple (es verdadera), se ejecuta el código asociado.

* Si la condición no se cumple (es falsa), el bloque de código se omite y el programa continúa con la siguiente instrucción.

#### - Ejemplo Práctico:

#### 📌📈Diagrama de Flujo:

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEiXf7tQxFTuBtCfWbij3eDzAfjUX_9J6D0GMkmOcV4k5QTgnNdpGvxtKP5jBCKae7wGt8-BK7D734NFf0aaRE6-z5_VWdlflTej_tyisG80NHzFRYIRkEpWRB4xlLC_dvgMUwh7hZHjWGfEHGxdTcmIEyZYB1QrV-a1ZIhGvfVeE2Ou9k4x-psDSlR1Snyk" alt="Descripción" width="70%">
</p>

#### ⚙️ Codigo en C

    #include <stdio.h>

    int main() {

    int edad;

    printf("Por favor, ingresa tu edad: ");
    scanf("%d", &edad);

    if (edad >= 18) {
        printf("Tienes %i anos, eres mayor de edad.\n", edad);
    }

    return 0;
    }
#### 🕵️ Explicación

Empezamos el algoritmo definiendo las variables, luego le pide al usuario que ingrese su edad, a continuación ingresamos la condición, que evalua si la edad del usuario es mayor o igual a 18 años. Si determina que sí lo es, ingresa a la derecha y muestra el mensaje de eres mayor de edad, continuando muestra tu edad y si eres mayor de edad.

Si determina que la edad ingresada es menor a 18, ignora el "if" y se cierra el algoritmo.

---

#### ✌️📖*ESTRUCTURA CONDICIONAL DOBLE (IF-ELSE)*

Es una estructura de control que permite a un programa tomar una decisión eligiendo entre dos caminos posibles. Funciona evaluando una condición.

* Si la condición se cumple (es Verdadera). Se ejecuta un bloque de instrucciones.

* Si no se cumple (es Falsa). Se ejecuta un bloque de instrucciones diferente.

#### - Ejemplo Práctico 

#### 📈📍Diagrama de Flujo 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEjr5F7C5qZeVC4I34e8zQ9ISCW4ohNHBThkouIDZMKzbRyFp3KS3Nqxw9lBx9wrXhODIzs6hODJwVIlkbxvki4dpeWYQy1IiG_HrWZC35KK87r_cqi5d9xwNeX94DpwylniG6NuB0fNGR3s9GW6vDQ-GgG_GUcVglDdLOLyVvHQeTf9LZZVNNd-eLqCGC29" alt="Descripción" width="70%">
</p>

#### 📎Codigo en C

    #include <stdio.h>
 
    int main (){
    
    int valor1,valor2,valor3,mayorvalor;

    printf("Ingrese el valor 1\n");
    scanf("%i", &valor1);
    getchar();

    printf("Ingrese el valor 2\n");
    scanf("%i", &valor2);
    getchar();

    printf("Ingrese el valor 3\n");
    scanf("%i",&valor3);
    getchar();

        if(valor1 > valor2){ 
            if (valor1 > valor3){

                mayorvalor = valor1;

            }else{ 

                mayorvalor = valor3;

            }
        }else if(valor2 > valor3){

            mayorvalor = valor2;

        }else{

            mayorvalor = valor3;
                
        }

    printf("El numero de mayor valor es: %i\n", mayorvalor);

    return 0;
    }

#### 🔗Explicación

Empezamos definiendo las variables, luego pedimos al usuario que ingrese 3 valores, luego la condición (if-else) evalua cual es el valor mayor de los 3 numeros ingresados.
Entramos al bloque si el valor2 es menor. El valor2 no puede ser el mayor. Ahora evaluamos entre valor1 y valor3. Si el 1 es mayor que 3, entonces valor1 es el mayor. Si el 1 no es mayor que 3, el  valor3 es el mayor.
Si valor1 no es mayor que valor2, significa que valor1 es menor. Ahora evaluamos entre valor2 y valor3. Si el 2 es mayor que el 3, valor2 es mayor. Si el 2 no no es mayor al 3, entonces valor3 es mayor.

---

#### 📋🗃️*ESTRUCTURA CONDICIONAL MULTIPLE (SWITCH)*

La estructura Switch es una herramienta de control que permite evaluar el valor de una variable o expresión y, en función de ese valor, elegir un único camino a seguir entre varias opciones posibles o tambien llamdas casos.

#### - Ejemplo Práctico

#### 📈🖇️Diagrama de flujo 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEgEN1YoJY-ERbg7nzZgW6WRUK-lfVNnwXCbXpj0g2SbgNYpJhSyEzgKlLQzBgdL4Bn8jMuZXu1s5UCCoWAhzT9fnzjvC-KHCVAOLIhBLZ4QxQbAXKlt01AW5fwkpgNEcAqLR7WEnZruw08b-N1Alu6KNYAmsYhwUJD_gGYulDNQijBmSsVcMXDGcb4KP2uu" alt="Descripción" width="70%">
</p>

#### 📑Codigo en C

    #include <stdio.h>

    int main (){

    int dia ;

    printf("Ingrese el dia de la semana en numero del 1 al 7:\n");
    scanf("%i", &dia);
    getchar ();

    switch(dia){

        case 1 :
          printf("Es lunes\n");
          break;
        case 2 :
            printf ("Es martes\n");
            break;
        case 3 :
            printf("Es miercoles\n");
            break;
        case 4 :
            printf("Es Jueves\n");
            break;
        case 5 :
            printf("Es viernes\n");
            break;
        case 6 :
            printf("Es sabado\n");
            break;
        case 7:
            printf("Es domingo\n");
            break; 
        default :
            printf("Numero no valido\n");
            break;                  
    }

    return 0;
    }

#### ⛓️‍💥Explicación

Primero definimos las variables, despues pedimos al usuario ingresar un numero del 1 al 7. Si el usuario escribe un el numero 1 la estructura analisa los diferentes casos hasta encontrar el caso 1 para poder mostrar el mensaje, por ejemplo si el usuario ingresa el numero 2 el algoritmo busca el caso 2 en este caso mostraria "Es martes".
Si ingresa un numero que no coincide con ningún caso, se le mostrara un mensaje que dice numero no valido.

--- 

### ♾️*ESTRUCTURAS REPETITIVAS*

---

#### ⌛🚀*ESTRUCTURA REPETITIVA (WHILE)*

El ciclo While o "mientras" es una estructura de control que permite repetir un bloque de instrucciones únicamente mientras su condición específica sea verdadera .

#### - Ejemplo Práctico

#### 📈🔎Diagrama de Flujo 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEgTy9lFL2QQBy2_6AUrHbh4WYYGsAKPMR4lpBaJpskl1GL_Ekq0YSYPk-dDIZzAN2-rQkVSxKomVytYDFKsqvTlUO_8AhaKz8NZtkP6DgwbKwXxtk889KELgDwX7zimmpxOif71tAgDghmg4lLVEZmg4hj9PEYGyFCq7xwrFYAEbHd4Rr7xcIv4P_h6GuCv" alt="Descripción" width="70%">
</p>

#### 🗄️Codigo en C

    #include <stdio.h>

    int main(){

    int contador = 0;
    int acumulador = 0;

    while(contador <= 5){

        acumulador = acumulador + contador;

        contador = contador + 1;

    }

    printf("El valor sumado es: %i\n",acumulador);

    return 0;
    }

#### 🧾Explicación

El funcionamiento del ciclo "While", lo que hace este programa es que el código dentro de las llaves { } se repetirá mientras la variable contador sea menor o igual a 5. Aumentamos el contador en 1. Si olvidamos esta línea, contador siempre sería 0, la condición siempre sería verdadera y el programa nunca terminaría creando un bucle infinito.

---

#### ✨🧠*ESTRUCTURA REPETITIVA (DO - WHILE)*

El Do-While es un ciclo repetitivo que ejecuta un bloque de código primero y evalúa la condición al final. Garantiza que las instrucciones se ejecuten al menos una vez, sin importar si la condición es verdadera o falsa desde el principio.

#### - Ejemplo Práctico 

#### 📈💯Diagrama de flujo 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEhevYLBaMUzWscX9di7sbd_CqGTBYGYoqzBM5NgIzS5IzXcfer8qWL30amQEK5k84ltuCd3GJD89wXPWe46B3olIyB_-EeXWSe6kTE_RtgTnGUrZg9YoIrpWEejGxs3U5sE2TFy6rv69iByx_E4Ox9_C2Mc9n2nZj0swt67OBdxYaCi90bCfNzNNiogKF20" alt="Descripción" width="70%">
</p>

#### 💻Codigo en C

    #include <stdio.h>

    int main() {

    int contador = 1;
    int resultado;
   
    do {
        
        resultado = 2 * contador;
        
        printf("2 x %2i = %i\n", contador, resultado);
        
        contador++; 
        
    } while (contador <= 12); 

    return 0;
    }
    
#### 👤Explicación

El código entra en un ciclo repetitivo. Multiplica 2 * contador y guarda el valor en resultado, Suma 1 al contador (contador++), por lo que ahora vale 2. Al final el programa muestra la tabla del 2 hasta el 12.

---

#### 💿🔍*ESTRUCTURA REPETITIVA (FOR)*

La estructura repetitiva "for" nos que permite ejecutar un bloque de código un número determinado de veces. A diferencia de otras estructuras repetitivas, el for es ideal cuando se conoce de antemano la cantidad exacta de iteraciones.

#### - Ejemplo Práctico

#### 📈🔩Diagrama de flujo

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEgPuskbkCBCcdi-AaPEjnOxPZaivM0QAMQV-_M13ND79dRo3GKusqrOYa5niS8nsEufA8-83XHJ6rLskVQZfhqF_-xnE0cH2Zfay78PmVeOCB74OrDs_doxFSwfaRGbYiGKoApZCr44qmA3vKlTmdL0_-dPuLXJ3SmNQKaKbaGF1d-UrgME_YsqO3Y0lJua" alt="Descripción" width="70%">
</p>

#### 💡Codigo en C

    #include <stdio.h>

    int main() {
    long numero;
    long contador;
    double factorial = 1; 

    printf("Ingrese un numero entero para calcular su factorial:\n");
    scanf("%ld", &numero);
    getchar();

    for (contador = 1; contador <= numero; contador++) {
        factorial = factorial * contador;
    }

    printf("El factorial de %ld es: %.0lf\n", numero, factorial);

    return 0;
    }

#### 👣Explicación

Utilizamos el ciclo "For", primero le pedimos al usuario que ingrese un numero para calcular su factorial entra en el círculo del for multiplicando repetidamente, y finalmente imprime el resultado mostrandonos el numero y el factorial.

--- 

### 📏🔔 *EJERCICIO COMBINADO ESTRUCTURA CONDICIONAL Y REPETITIVA*

---

#### 📰Descripción del Problema

Desarrollar un algoritmo que permita calcular el rendimiento académico de un estudiante basándose en un conjunto variable de evaluaciones y determinar su situación final en la materia, utilzando estructuras condicionales y repetitivas en el lenguaje python.

#### - Ejemplo Práctico

#### 📁📈Diagrama de Flujo

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEjXbVU_BhwxCovlk_rbxS_3avM_eNR-GOurtwaq0iF1bNwhMhumY7i7Jcox81ObCG_dnCG5-xcxHQKkAAJWzHr4txtx6IsJfwPbOAtH2c6LLzjZ_BFkz6_b9Q_ragRd2zGpvjFngHP6iURXUiWLjM0CcJssQT3af3a581xmXpV0ptCrOKgAaBMN0cuvEiKt" alt="Descripción" width="70%">
</p>

#### ⚒️Codigo en Python 

    alumno = input("Ingresa el nombre del alumno:\n")
    cantidad = int(input("Ingrese la cantidad de notas:\n"))

    suma_total = 0.0

    print(f"Ingresando notas de {alumno}")

    for i in range(cantidad):

    nota = float(input(f"Ingresa la nota {i + 1}: "))
    
    suma_total = suma_total + nota 

    if cantidad > 0:
        promedio = suma_total / cantidad
    else:
        promedio = 0


    if promedio >= 7:
        estado_final = "Aprobado"
    else:
        estado_final = "Reprobado"

    print(f"Alumno: {alumno}")
    print(f"Promedio final: {promedio:.2f}") 
    print(f"Estado: {estado_final}")

#### 📂Verificación 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEhU495E0DoviYYCU0OH2_xQo-8cs4ZZP61PLuVDm-THDOCn256okV5EJgr4pGDSuoF9ewbDqlqQn0nSIbzR3v6ApxtOCD74Lc-ZpRPVArJxHs6u2lblKvSE2du1R4BBALGdDfOZQRY93mrYzl53xJQkwPlYy27ocMg7iFA7OgH_VzQnMWwJlWCnZSaLynmo" alt="Descripción" width="70%">
</p>

---

###  📑⚙️*PRINCIPALES DIFICULTADES EN LA APLICACIÓN DE LOS CONTENIDOS*

Se me dificultó un poco aprender cuando se aplicaba cada estructura, bien sea condicional o repetitiva, tambien se me hizo complicado de aprender las restricciones y sintaxis de estas, ademas el cambio a el lenguaje de java se me dificulto un poco porque estaba acostumbrado a el lenguaje de C entonces su estructura se me hizo confusa.

--- 

### 🧠🤵*REFLEXIÓN CRÍTICA DE LOS APRENDIZAJES DE LA UNIDAD*

En esta unidad aprendimos a como utilizar las estructuras repetitivas y condicionales, ya que estas ayudan a optimizar y dinamizar el código. Ha sido de gran ayuda para saber cuando es necesario aplicar las diferentes estructuras ya sea repetitiva o condicional, aunque esta se me haya dificultado un poco.

<p align="right">
  <a href="index.md">Volver a la página principal</a>
</p>
