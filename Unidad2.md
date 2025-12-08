# ⚛️ CONTENIDO UNIDAD 2

---

### *ESTRUCTURAS CONDICIONALES*

---

### *ESTRUCTURA CONDICIONAL SIMPLE (IF)*

La estructura condicional simple (IF) es una herramienta de programación que permite ejecutar un bloque de código solo si una condición específica es verdadera [1].

* Si la condición dentro del if se cumple (es verdadera), se ejecuta el código asociado.

* Si la condición no se cumple (es falsa), el bloque de código se omite y el programa continúa con la siguiente instrucción.

#### - Ejemplo Práctico:

#### Diagrama de Flujo:

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEiXf7tQxFTuBtCfWbij3eDzAfjUX_9J6D0GMkmOcV4k5QTgnNdpGvxtKP5jBCKae7wGt8-BK7D734NFf0aaRE6-z5_VWdlflTej_tyisG80NHzFRYIRkEpWRB4xlLC_dvgMUwh7hZHjWGfEHGxdTcmIEyZYB1QrV-a1ZIhGvfVeE2Ou9k4x-psDSlR1Snyk" alt="Descripción" width="70%">
</p>

#### Codigo en C

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
#### Explicación

Empezamos el algoritmo definiendo las variables, luego le pide al usuario que ingrese su edad, a continuación ingresamos la condición, que evalua si la edad del usuario es mayor o igual a 18 años. Si determina que sí lo es, ingresa a la derecha y muestra el mensaje de eres mayor de edad, continuando muestra tu edad y si eres mayor de edad.

Si determina que la edad ingresada es menor a 18, ignora el "if" y se cierra el algoritmo.

---

#### *ESTRUCTURA CONDICIONAL DOBLE (IF-ELSE)*

Es una estructura de control que permite a un programa tomar una decisión eligiendo entre dos caminos posibles. Funciona evaluando una condición [2].

* Si la condición se cumple (es Verdadera). Se ejecuta un bloque de instrucciones.

* Si no se cumple (es Falsa). Se ejecuta un bloque de instrucciones diferente.

#### - Ejemplo Práctico 

#### Diagrama de Flujo 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEjr5F7C5qZeVC4I34e8zQ9ISCW4ohNHBThkouIDZMKzbRyFp3KS3Nqxw9lBx9wrXhODIzs6hODJwVIlkbxvki4dpeWYQy1IiG_HrWZC35KK87r_cqi5d9xwNeX94DpwylniG6NuB0fNGR3s9GW6vDQ-GgG_GUcVglDdLOLyVvHQeTf9LZZVNNd-eLqCGC29" alt="Descripción" width="70%">
</p>

#### Codigo en C

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

#### Explicación

Empezamos definiendo las variables, luego pedimos al usuario que ingrese 3 valores, luego la condición (if-else) evalua cual es el valor mayor de los 3 numeros ingresados.
Entramos al bloque si el valor2 es menor. El valor2 no puede ser el mayor. Ahora evaluamos entre valor1 y valor3. Si el 1 es mayor que 3, entonces valor1 es el mayor. Si el 1 no es mayor que 3, el  valor3 es el mayor.
Si valor1 no es mayor que valor2, significa que valor1 es menor. Ahora evaluamos entre valor2 y valor3. Si el 2 es mayor que el 3, valor2 es mayor. Si el 2 no no es mayor al 3, entonces valor3 es mayor.

---

#### *ESTRUCTURA CONDICIONAL MULTIPLE (SWITCH)*

La estructura Switch es una herramienta de control que permite evaluar el valor de una variable o expresión y, en función de ese valor, elegir un único camino a seguir entre varias opciones posibles o tambien llamdas casos [3].

#### - Ejemplo Práctico

#### Diagrama de flujo 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEgEN1YoJY-ERbg7nzZgW6WRUK-lfVNnwXCbXpj0g2SbgNYpJhSyEzgKlLQzBgdL4Bn8jMuZXu1s5UCCoWAhzT9fnzjvC-KHCVAOLIhBLZ4QxQbAXKlt01AW5fwkpgNEcAqLR7WEnZruw08b-N1Alu6KNYAmsYhwUJD_gGYulDNQijBmSsVcMXDGcb4KP2uu" alt="Descripción" width="70%">
</p>

#### Codigo en C

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

Primero definimos las variables, despues pedimos al usuario ingresar un numero del 1 al 7. Si el usuario escribe un el numero 1 la estructura analisa los diferentes casos hasta encontrar el caso 1 para poder mostrar el mensaje, por ejemplo si el usuario ingresa el numero 2 el algoritmo busca el caso 2 en este caso mostraria "Es martes".
Si ingresa un numero que no coincide con ningún caso, se le mostrara un mensaje que dice numero no valido.

--- 

### *ESTRUCTURAS REPETITIVAS*

---

#### *ESTRUCTURA REPETITIVA (WHILE)*

El ciclo While o "mientras" es una estructura de control que permite repetir un bloque de instrucciones únicamente mientras su condición específica sea verdadera [2].

#### - Ejemplo Práctico

#### Diagrama de Flujo 

<p align="left">
  <img src="https://blogger.googleusercontent.com/img/a/AVvXsEgTy9lFL2QQBy2_6AUrHbh4WYYGsAKPMR4lpBaJpskl1GL_Ekq0YSYPk-dDIZzAN2-rQkVSxKomVytYDFKsqvTlUO_8AhaKz8NZtkP6DgwbKwXxtk889KELgDwX7zimmpxOif71tAgDghmg4lLVEZmg4hj9PEYGyFCq7xwrFYAEbHd4Rr7xcIv4P_h6GuCv" alt="Descripción" width="70%">
</p>

#### Codigo en C

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

#### Explicación

El funcionamiento del ciclo "While", lo que hace este programa es que el código dentro de las llaves { } se repetirá mientras la variable contador sea menor o igual a 5. Aumentamos el contador en 1. Si olvidamos esta línea, contador siempre sería 0, la condición siempre sería verdadera y el programa nunca terminaría creando un bucle infinito.







