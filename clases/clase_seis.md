# Modulacion (Modificar una propiedad de una señal portadora)
f(t) × g(t)

# Convolucion
1/2pi × (F(⍵)×G(⍵))

# Calculo de longitud de onda en el vacio
ƛ = c / f

# Por que modular la frecuencia
Si yo quiero transmitir una onda, necesito modular la portadora para colocarle la informacion 
adentro y ademas desplazar ese espectro para poder tener una longitud de onda que pueda ser facilmente transmitida
por un transmisor de un tamaño considerable (ver calculo de longitud de onda)

# AM (Amplitud Modulada)
* Portadora Suprimida
* Portadora Vestigial
* Portadora

# FM (Frecuencia Modulada)
La frecuencia de la señal portadora es proporcional a la señal de la informacion

# PM (Fase Modulada [Phase])
La fase de la señal portadora es proporcional a la señal de la informacion

# Informacion y Canales

|Señal\Info|Analogico|Digital|
|----------|---------|-------|
|Analogico |AM       |ASK    |
|          |FM       |FSK    |
|          |PM       |PSK    |
|----------|---------|-------|
|Digital   |         |       |
|----------|---------|-------|

> SK = Shift Keying


## ASK
* Donde hay un 1 dejo pasar la portadora
* Donde hay un 0 no dejo pasar la portadora

> O al reves

### Problemas
* El circuito receptor puede perderse cuando se pierde la señal y se genera
un defasaje.

Para eliminar este problema, se deja pasar a la portadora en todo momento,
pero con amplitud notablemente menor.

Por ende la amplitud es la que define el dato

Pueden enviarse multiples niveles para codificar mayor cantidad de informacion

## FSK
* Donde hay un 1 utilizo una frecuencia
* Donde hay un 0 utilizo otra frecuencia

## PSK
* Donde hay un 1 utilizo fase 0
* Donde hay un 0 utilizo fase pi

> Se puede utilizar cualquier otra fase que resulte comoda

-----------------

Tanto en ASK, FSK y PSK, se pueden agregar mayor cantidad de variaciones
para codificar mayor cantidad de datos en la misma señal

Para lograr esto, se utilizan combinaciones entre ellas, por ejemplo,
fase y amplitud

> Ejemplos son QAM y QPSK
