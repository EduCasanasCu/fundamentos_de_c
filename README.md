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
