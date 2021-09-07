# ***Roscadora de Bornes***

## Descripción:

La maquina de estado a realizar es en base a una roscadora de bornes. Esta misma estará subdividida en 5 estados diferentes:

- El primer estado (inicialización):Consistirá en la inicialización de los sensores y la carga de los bornes.
- El segundo estado (posición): Trabajará en la inserción del borne en la zona de roscado.
- El tercer estado (roscado): Se encargará de roscar el borne, finalizando la tarea cuando rosque una distancia "x" determinada por el usuario.
- El cuarto estado (desenroscado): Cumplirá la tarea de desenroscar el macho del borne, permitiendo la futura salida del mismo.
- El quinto estado(sustracción): Realizará la tarea de remover el borne roscado, permitiendo asi la inserción de un nuevo borne y repitiendo el poceso desde el segundo estado
