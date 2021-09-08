# ***Roscadora de Bornes***

## Descripción:

La maquina de estado a realizar es en base a una roscadora de bornes. Esta misma estará subdividida en 5 estados diferentes:

- El primer estado (inicialización):Consistirá en la inicialización de los sensores y la carga de los bornes.
- El segundo estado (posición): Trabajará en la inserción del borne en la zona de roscado.
- El tercer estado (roscado): Se encargará de roscar el borne, finalizando la tarea cuando rosque una distancia "x" determinada por el usuario.
- El cuarto estado (desenroscado): Cumplirá la tarea de desenroscar el macho del borne, permitiendo la futura salida del mismo.
- El quinto estado(sustracción): Realizará la tarea de remover el borne roscado, permitiendo asi la inserción de un nuevo borne y repitiendo el poceso desde el segundo estado

```c
/*carpeta lib.h donde declaro los prototipos de las funciones*/
#ifndef LIB_H
#define LIB_H
#include <stdio.h>

/*
*Función: init()
*Prototipo de funcion init, no requiere parámetros, se encarga de inicializar los sensores, determinar la distancia a roscar y cargar los bornes 
*@params:(void).
*@returns: int devuelve un "1" cuando esten inicializados los sensores y cargados los bornes
*/
int(init)(void);

/*
*Función: posicion()
*Prototipo de función posicion, no requiere parámetros, se encarga de posicionar el borne para su futuro roscado
*@params:(void).
*@returns: int devuelve un "1" cuando esté correctamente posicionado el borne (determinado por un sensor en la base)
*/
int(posicion)(void);

/*
*Función: roscado()
*Prototipo de función roscado, no requiere parámetros, su función es roscar el borne una cierta distancia ya establecida
*@params:(void).
*@returns: int devuelve un "0" cuando haya llegado al tope de roscado
*/
int(roscado)(void);

/*
*Función: desenrosca()
*Prototipo de función desenrosca, no requiere parámetros, desenrosca una distancia determinada para la salida del borne
*@params:(void).
*@returns: int devuelve un "1" cuando haya llegado al tope de desenroscado 
*/
int(desenrosca)(void);

/*
*Función:sustitución()
*Prototipo de función sustitucion, no requiere parámetros, remueve el borne roscado, dejando espacio para el nuevo borne
*@params:(void).
*@returns: int devuelve un "0" cuando el borne haya sido sustraido
*/
int(sustitucion)(void);

/*puntero a funciones*/
int(*estados[])(void);

#endif
```

```c
/*Carpeta funciones.c donde se realizan las funciones*/
#include lib.h

int(init)(void)
{

}
int(posicion)(void);
{

}
int(roscado)(void);
{

}
int(desenrosca)(void);
{

}
int(sustitucion)(void);
{

}
```