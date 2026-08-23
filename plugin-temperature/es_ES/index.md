# Complemento de temperatura

<img src="{{site.baseurl}}/plugin-temperature/{{site.img}}/temperature_icon.png" class="pluginLogo" width="100" />

## Descripción

Este complemento permite calcular el efecto del viento sobre la temperatura percibida (windchill, sobre todo cuando las temperaturas son bajas), así como la sensación de incomodidad provocada por el índice de humedad cuando las temperaturas son elevadas (humidex).

## Configuración

El complemento no tiene configuración general.
Hay que instalar dispositivos para medir la temperatura, la humedad y la velocidad del viento.
Se puede indicar:

- Un umbral de alerta para el índice de calor (HUMIDEX). Por defecto, la alerta se activa a partir de los 40 °C.
- Un umbral de prealerta para el índice de calor (HUMIDEX). Por defecto, la prealerta se activa a partir de los 30 °C.

## Temperaturas percibidas

> Fuentes:
>
> - <a href="https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul">https://fr.m.wikipedia.org/wiki/Refroidissement_éolien#Calcul</a>
> - <a href="http://www.meteo-mussidan.fr/hum.php">http://www.meteo-mussidan.fr/hum.php</a>

| Mensaje digital | Mensaje |
| :---------------: | :----------------------------------------------------------------------------------------------------------------- |
|     <b>-7</b>     | ¡Peligro! Riesgo extremadamente alto de congelación en menos de 2 minutos (véase la nota) y de hipotermia. Permanece a resguardo |
|     <b>-6</b>     | Riesgo muy elevado de congelación en un plazo de 2 a 5 minutos (véase la nota) sin protección integral ni actividad |
|     <b>-5</b>     | Alto riesgo de congelación en 5 a 10 minutos (véase la nota) de la piel expuesta y de hipotermia |
|     <b>-4</b>     | Riesgo moderado de congelación de la piel expuesta en un plazo de entre 10 y 30 minutos y de hipotermia |
|     <b>-3</b>     | Bajo riesgo de congelación e hipotermia |
|     <b>-2</b>     | Bajo riesgo de heladas |
|     <b>-1</b>     | Sin riesgo de congelación ni hipotermia (en condiciones normales de exposición) |
|     <b>1</b> | Sensación de frescor o frío |
|     <b>2</b> | Sin molestias |
|     <b>3</b> | Sensación de bienestar |
|     <b>4</b> | Sensación de malestar más o menos intensa |
|     <b>5</b> | Sensación de incomodidad bastante intensa. Se recomienda precaución. Reducir el ritmo de ciertas actividades al aire libre. |
|     <b>6</b> | Sensación generalizada de malestar. Peligro. Evitar el esfuerzo. |
|     <b>7</b> | Peligro extremo. Paro laboral en numerosos sectores. |
|     <b>8</b> | Golpe de calor inminente (peligro de muerte). |
