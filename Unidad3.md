## 📝 UNIDAD 3

###  MODULARIDAD

---

#### 📋Pase de párametro por Valor

---

Este método consiste en crear una copia del valor de una variable y pasar esa copia a la función.
Cualquier modificación que se haga dentro de la función afecta solo a esa copia, por lo que la variable original queda intacta y no sufre ningún cambio, ya que está fuera del ámbito de la función.

#### 🧑‍💻 Ejemplo:

##### Código en C:

```
#include <stdio.h>

void duplicar(int n) {
    n = n * 2; 
    printf("Valor dentro de la funcion: %d\n", n);
}

int main() {
    int numero = 10;

    duplicar(numero);

    printf("Valor en el main (original): %d\n", numero);

    return 0;
}
```

#### 💡Explicación:

En el main se crea la variable numero y se le pone 10, o sea, se reserva un pedacito de memoria con ese valor. Cuando llamamos a duplicar (numero), lo que pasa es que el programa no le pasa la variable original, sino que hace una copia del valor (el 10) y esa copia llega a la función como la variable local n. Entonces n empieza valiendo 10, pero dentro de la función le cambiamos el valor y pasa a valer 20. Ahí se imprime el 20, todo bien. Pero cuando la función termina, esa variable n desaparece junto con su pedacito de memoria. Entonces volvemos al main y la variable numero sigue siendo exactamente la misma de antes, con su 10 original, porque nunca la tocamos. Lo que se modificó fue solo la copia que estaba dentro de la función.

---

#### 📍Pase de párametro por Referencia

---

En este caso no mandamos copias del valor, sino que le pasamos directamente la dirección de memoria donde está guardada la variable original. Gracias a eso, la función no trabaja con una fotocopia, sino que accede al mismo lugar en la memoria y puede cambiar el valor de verdad. En C esto se hace con punteros: usamos el & para sacar la dirección y el * para decir “quiero trabajar con lo que hay en esa dirección”.

#### 🧑‍💻 Ejemplo:

##### Código en C:

```

#include <stdio.h>

void duplicar(int *n) {
    *n = *n * 2;
    printf("Valor dentro de la funcion (modificando el original): %d\n", *n);
}

int main() {
    int numero = 10;

    duplicar(&numero);

    printf("Valor en el main (ya cambio): %d\n", numero);

    return 0;
}

```

#### 💡Explicación:

En el ejemplo, la función se declara como void duplicar(int *n), indicando que recibirá la dirección de memoria de una variable (el asterisco * señala que es un puntero).Luego, en el main, al invocar la función con duplicar(&numero), el operador & entrega precisamente la ubicación en memoria donde está almacenada la variable numero. Dentro de la función, la línea *n = *n * 2 significa “ve a la dirección de memoria que me pasaron, toma el valor que está allí, multiplícalo por 2 y guarda el resultado en el mismo lugar”. De esta forma, la modificación se realiza directamente en la memoria original de la variable, por lo que al finalizar la función, el valor de numero en el main ya ha cambiado sin necesidad de devolver nada.

---

### 🗄️ARREGLOS

---

#### 📏 Arreglo Unidimensional 

---

Este tipo de arreglos se caracteriza por contener una única fila y múltiples columnas, formando una estructura lineal conocida como arreglo unidimensional o vector. Las posiciones dentro de este arreglo comienzan desde cero y a cada una de ellas se le denomina índice. Los índices permiten acceder de manera rápida y directa a cualquier elemento del arreglo mediante su posición numérica.

#### 🧑‍💻 Ejemplo:

##### Código en C:

```

#include <stdio.h>

int main() {

    int numeros[5] = {10, 20, 30, 40, 50};

    printf("El primer numero es: %d\n", numeros[0]);

    for (int i = 0; i < 5; i++) {
        printf("Indice %d: Valor %d\n", i, numeros[i]);
    }

    return 0;
}

```
#### 💡Explicación:

Al escribir int numeros [5], creas una fila de 5 casilleros en la memoria del sistema, todos pegados uno tras otro. El programa le asigna un número de etiqueta (índice) a cada casillero,que empieza siempre desde el 0 para que la computadora sepa exactamente dónde buscar cada dato. Usamos el for, para activar un contador automático que va saltando de casillero en casillero. En cada salto, el programa abre el casillero correspondiente al número del contador, toma el valor que guardamos ahí y lo muestra, repitiendo esto hasta llegar al último espacio reservado.

---

#### 🗓️ Arreglo Bidimensional

---

Este tipo de arreglo se caracteriza por tener múltiples filas y columnas, y se denota como m[i][j], siendo i el índice de la fila y j el índice de la columna.

#### 🧑‍💻 Ejemplo:

##### Código en C:

```

#include <stdio.h>

int main() {

    int matriz[3][3] = {
        {1, 2, 3}, 
        {4, 5, 6}, 
        {7, 8, 9}  
    };

    printf("Contenido de la matriz:\n");

    for (int i = 0; i < 3; i++) { 
        for (int j = 0; j < 3; j++) { 
            printf("%d ", matriz[i][j]);
        }
        printf("\n"); 
    }

    return 0;
}

```

#### 💡Explicación:

Comenzamos declarando la matriz con int matriz[3][3], donde el primer número define las filas y el segundo las columnas, reservando un total de 9 espacios para enteros. Al inicializarla con llaves, cada par de llaves internas representa una fila completa. El primer ciclo for se posiciona en una fila, y mientras se queda ahí, el segundo ciclo for recorre cada columna de esa fila para imprimir el valor con printf. Al terminar cada fila, se usa un printf("\n") para dar un salto de línea y mantener la forma visual de tabla.

---

#### 🧊 Arreglo Tridimensional 

---

Este arreglo se distingue porque posee profundidad, filas y columnas; lo representamos mediante m[i,j,k], siendo i el índice de profundidad, j el que marca las filas y k las columnas.

#### 🧑‍💻 Ejemplo:

##### Código en C:

``` 
#include <stdio.h>

int main() {

    int inventario[2][2][2] = {
        {
            {15, 20}, 
            {10,  5}  
        }, 
        {
            {40, 33}, 
            {12, 18}  
        }  
    };


    for (int i = 0; i < 2; i++) {        
        printf("\nPASILLO %d:", i);
        
        for (int j = 0; j < 2; j++) {     
            printf("\n  Estante %d -> ", j);
            
            for (int k = 0; k < 2; k++) { 
                printf("[Caja %d: %d unidades]  ", k, inventario[i][j][k]);
            }
        }
        printf("\n"); 
    }

    return 0;
}

```

#### 💡Explicación:

La primera dimensión representa los bloques grandes (Pasillos), la segunda las filas (Estantes) y la tercera los elementos individuales (Cajas). Al declarar int inventario[2][2][2], creamos una estructura que contiene un total de 8 espacios. Para llenarlo o leerlo, utilizamos tres ciclos for anidados: el primero selecciona el pasillo, el segundo el estante y el tercero la caja; esta combinación de índices funciona como una coordenada exacta que permite al programa saber exactamente en qué rincón de la memoria está guardado cada valor

---

### 🤔 PRINCIPALES DIFICULTADES EN LA APLICACIÓN DE LOS CONTENIDOS

Se me dificulto un poco aprender los pases por referencia y por valor, como se debe usar los punteros para hacer los pases por referencia a su vez también se me dificulo como invocar funciones.

---

### 🧠💡 REFLEXIÓN CRÍTICA DE LOS APRENDIZAJES DE LA UNIDAD 

La unidad me permitió darme cuenta de lo fundamental que es pasar de una programación básica y desordenada a una programación lógica, estructurada y bien organizada. Además, el manejo de la memoria mediante punteros y la organización de datos con arreglos multidimensionales son conocimientos que me serán muy valioso

---

<p align="right">
  <a href="index.md">Volver a la página principal</a>
</p>




