# Fundamentos de C

## Estructura inicial de un programa en C

```c
#include <stdio.h>
int main(){
    
    return 0;
}
```
## Comentarios
```c
// este es un comentario de una línea

/* Este es un comentario
de múltiples
líneas
*/
```
## Caracteres de modificación

| %c | unico caracter |
|:------:|:--------:|
| %d | entero |
| %u | entero sin signo en base decimal |
| %o | entero en base octal |
| %x | entero en base hexadecimal |
| %e | un numero real en coma flotante, con exponente |
| %f | un numero real en coma flotante, sin exponente |
| %s | una cadena de caracteres |
| %p | puntero o direccion de memoria |

## Variables Enteras y mostrar por consola
```c
#include <stdio.h>
int main(){

    int edad = 25;
    int edad2 = 33;

    printf("La segunda edad es: %d \nLa primera edad es: %d", edad2, edad);

    return 0;
}
```
**Salida por consola:**
```
La segunda edad es: 33 
La primera edad es: 25
``` 
## Variables constantes y flotantes
```c
#include <stdio.h>
int main(){
    // Constantes => #define NOMBRE valor
    #define PI 3.1416

    // Variables => tipo nombre = valor;
    float sueldo = 102500;
    float bono = 450;

    sueldo = sueldo + bono; // sueldo += bono;

    printf("El sueldo es: %f\n", sueldo);
    printf("El valor de PI es: %f", PI);

    return 0;
}
```
**Salida por consola:**
```
El sueldo es: 102950.000000
El valor de PI es: 3.141600
```
## Secuencias de escape
| \0 | nulo |
|:------:|:--------:|
| \b | retroceso |
| \t | tabulador |
| \n | salto de línea |
| \f | salto de pagina |
| \r | retorno de carro |
| \\" | comillas |
| \\? | signo de interrogacion |
| \\\\ | barra invertida |
## Utilizacion de las secuencias de escape
```c
#include <stdio.h>
int main(){
    // salto de linea
    printf("Hello, World!\n");

    // tabulador
    printf("Buenos\tdias");

    // comillas
    printf("\n\"Buenos dias\"");
    
    return 0;
}
``` 
**Salida por consola:**
```
Hello, World!
Buenos  dias
"Buenos dias"
``` 
## Operadores aritmeticos
```c
#include <stdio.h>
int main(){
    
    int num1 = 10;
    int num2 = 5;
    int suma, resta, multiplicacion, division, modulo;

    //Suma
    suma = num1 + num2;
    printf("Suma: %d\n", suma);

    //Resta
    resta = num1 - num2;
    printf("Resta: %d\n", resta);

    //Multiplicación
    multiplicacion = num1 * num2;
    printf("Multiplicación: %d\n", multiplicacion);

    //División
    division = num1 / num2;
    printf("División: %d\n", division);

    //Módulo
    modulo = num1 % num2;
    printf("Módulo: %d\n", modulo); 
    
    return 0;
}
```
**Salida por consola:**
```
Suma: 15
Resta: 5
Multiplicación: 50
División: 2
Módulo: 0
```
## Operadores de incremento y decremento
### Incremento
```c
#include <stdio.h>
int main(){
    
    int numero = 5;
    int numero2 = 10;

    numero++;
    numero2 += 1;

    printf("El numero incrementado es: %d\n", numero);
    printf("El numero2 incrementado es: %d\n", numero2);
    
    return 0;
}
```
**Salida por consola:**
```
El numero incrementado es: 6
El numero2 incrementado es: 11
```
### Decremento
```c
#include <stdio.h>
int main(){
    
    int numero = 15;
    int numero2 = 20;

    numero--;
    numero2 -= 10;

    printf("El numero decrementado es: %d\n", numero);
    printf("El numero2 decrementado es: %d\n", numero2);
    
    return 0;
}
```
**Salida por consola:**
```
El numero decrementado es: 14
El numero2 decrementado es: 10
```
