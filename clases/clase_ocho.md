# Ruido
## Clasificaciones
### Respecto del equipo
* Interno
* * Termico: Propio de la naturaleza - Proporcional a la temperatura
* * Granalla: Discontinuidad de la conductividad del equipo (el equipo no es perfecto)
* Externo: Cualquier otro equipo, la red, electricidad, etc

## Figura de Ruido
La relacion entre las relaciones Señal/Ruido entre la entrada y la salida del equipo

Referencias:
> Si = Input Signal
> So = Output Signal
> Ni = Input Noise
> No = Output Noise
> Na = Device (Amplifier) Noise
> G = Gain

Calculo de la señal de salida
> So = Si x G
> No = Ni x G + Na

Deduccion de la formula de la Figura de ruido:
> F = (Si/Ni) / (So/No) = (Si/Ni) x (No/So)
> F = (Si/Ni) x ((Ni x G + Na)/(Si x G))
> F = ((Ni x G)/(Ni x G)) + Na/(Ni x G)
> F = 1 + Na/(Ni x G)

Conclusion
> Si uno debe mejorar la señal, la etapa mas critica es la de generacion, ya
> que siempre hay mayor cantidad de ruido a lo largo de la transmision de una
> señal

# Señales digitales

|Señal\Info|Analogico|Digital                   |
|----------|---------|--------------------------|
|Analogico |AM       |ASK                       |
|          |FM       |FSK                       |
|          |PM       |PSK                       |
|          |PAM      |                          |
|          |PWM      |                          |
|          |PPM      |                          |
|----------|---------|--------------------------|
|Digital   |PCM      |Codificacion en banda base|
|----------|---------|--------------------------|

## PAM (Modulacion por alto de pulsos) [Analogica]
Se realiza un muestreo de la señal (en un sampling rate, utilizando un tren de deltas)
La información se transmite a partir de la amplitud de los puntos muestreados

> Teorema del Muestreo
> fs >= 2 fmax

* PAM Natural: en lugar de deltas se utilizan pulsos y se copia la onda en pequeños segmentos
* PAM "Cresta Plana": Como PAM Natural, pero en lugar de copiar el segmento se
                      mantiene el valor de amplitud inicial a lo largo de la muestra

### PWM (Width)
A partir de PAM, transforma la relacion de amplitudes en anchos de pulso de la misma amplitud

### PPM (Position)
A partir de PAM, transformo la relacion de amplitudes en una posicion en el tiempo,
los pulsos tienen ancho y alto fijo

## PCM (Pulse Code Modulation)

Filtro -> Muestreo -> Cuantifico -> Codifico

### Cuantificacion
Asignar cotas de valor para segmentos de altura y transformar la señal en valores discretos


