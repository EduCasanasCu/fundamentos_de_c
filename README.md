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
