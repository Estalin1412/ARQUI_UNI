# Historia de computadores
### CPU
unidad de procesador central
Para realizar operaciones lógicas dentro del procesador, para el dezplazamiento de bits
## Microcontrolador
Manejo de puertos, iterrupciones, timers, etc.

## ROM
 memoria dde solo lectura
## RAM
 Memoria de acceso a los datos

# Lenguaje ensamblador
## Directivas
Proporcionan informacion del programa
## Descriptores de datos
Para definir valores
# Instrucciones ejecutables

## Linea de intruciones
campo etiqueta:
campo operando: Nombre de los registros
Instrucciones: 

## Modos de direccionamiento
La forma en que sea acceden a los datos, determinan como el byte del operador es seleccionado
* MOV A,B; lo de B lo paso a A
* MOV 30H, A;  
## ReEGISTRO DE FUNCIONES
Posiciones de memoria que esta dentro del chip
## ejemplo 

```
org oh
mov 40h, #11h
mov 41h, #16h
mov A, 40h  ; Muevo a A en valor de 40h
add A, 41h  ; Sumo A + 41h y guardo en 41h
mov 42h, A
sjmp $ ; Salta el contro así mismo

```
## Para encender o pagar led
```
org 0h
repite:
    setb P1, 0
    nop
    nop
    clr P1. 0
    nop
    nop
    sjmp repite
```