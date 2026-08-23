# Complemento «Rosée» - «Givre» - «Tendance»

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

# Descripción

Este complemento permite conocer el punto de rocío para saber si la hierba estará mojada por la mañana o, en invierno, si habrá que raspar el parabrisas.
Para que funcione, hay que indicar un dispositivo de temperatura y otro de humedad (exteriores, por supuesto…).
También es posible calcular la tendencia meteorológica futura basándose en la evolución del tiempo.

# Configuración

El complemento no tiene configuración general, hay que:

> Elige un método de cálculo:

    - Humedad absoluta
    - Punto de escarcha
    - Punto de rocío
    - Punto de rocío y punto de escarcha
    - Tendencias meteorológicas
    - Temperaturas percibidas

> Rellena los campos obligatorios según el método de cálculo:

    - Equipos de «Temperatura» (°C)
    - Equipo «Humedad relativa» (%)
    - Equipo «Vitesse du Vent»
    - Parámetro «Presión atmosférica» (hPa): este campo es obligatorio para el método de cálculo «Tendencia meteorológica» y debe tener el historial activado y la opción «Repetir valores idénticos» en «Sí». Para los demás cálculos, el valor se establece en 1013,25 hPa si no se introduce ningún dato.

<b>Opcional: </b>

> - Umbral de la alerta de rocío (°C): umbral de activación de la alerta de rocío, 2 °C por defecto (disminución del punto de rocío T°-Tr°). Se debe ajustar en función de las observaciones locales.
> - Umbral de humedad absoluta: umbral de humedad absoluta por debajo del cual es poco probable que se forme escarcha; el valor por defecto es 2,8.
> - Compensación de temperatura: Se debe ajustar en función de las observaciones locales y de la posición del sensor; el valor por defecto es 0.

# Alerta de heladas

> Fuentes:
>
> - <a href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/</a>

El complemento calcula cuatro niveles de alerta:

|  Casos  | Información |
| :---: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **0** | - Cálculo: No se da ninguno de los casos siguientes<br/>- Alerta de hielo: 0<br/>- Alerta de rocío: Automática<br/>- Mensaje numérico de hielo: 0<br/>- Mensaje informativo: No hay riesgo de formación de hielo |
| **1** | - Cálculo: (Temperatura <=1 y Punto de escarcha <= 0) y (Humedad absoluta en (gr/m³) < Umbral de humedad absoluta)<br/>- Alerta de escarcha: 1<br/>- Alerta de rocío: forzada a 0<br/>- Mensaje numérico: 1<br/>- Mensaje: Es poco probable que se forme escarcha a pesar de la temperatura |
| **2** | - Cálculo: (Temperatura <=4 y Punto de escarcha <= 0,5)<br/>- Alerta de escarcha: 1<br/>- Alerta de rocío: forzada a 0<br/>- Mensaje numérico: 2<br/>- Mensaje: Riesgo de escarcha |
| **3** | - Cálculo: (Temperatura <=1 y Punto de escarcha <= 0) y (Humedad absoluta en (gr/m3) > Umbral de humedad absoluta)<br/>- Alerta de escarcha: 1<br/>- Alerta de rocío: forzada a 0<br/>- Mensaje numérico: 3<br/>- Mensaje: Escarcha, Presencia de escarcha |

# Tendencias meteorológicas

> Fuentes:
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

El complemento calcula seis niveles de información:

|  Nivel  | Tendencia | Imagen del widget |
| :------: | :--------------------------------- | :----------------------------------------------------------------------: |
| <b>0</b> | Fuerte deterioro, inestable | <img src="../{{site.img}}/tendance_0.png" alt="Tendencia 0" width="40" /> |
| <b>1</b> | Deterioro, mal tiempo prolongado | <img src="../{{site.img}}/tendance_1.png" alt="Tendencia 1" width="40" /> |
| <b>2</b> | Deterioro lento, tiempo estable    | <img src="../{{site.img}}/tendance_2.png" alt="Tendencia 2" width="40" /> |
| <b>3</b> | Mejora gradual, tiempo estable   | <img src="../{{site.img}}/tendance_3.png" alt="Tendencia 3" width="40" /> |
| <b>4</b> | Mejora, buen tiempo duradero   | <img src="../{{site.img}}/tendance_4.png" alt="Tendencia 4" width="40" /> |
| <b>5</b> | Fuerte repunte, inestable | <img src="../{{site.img}}/tendance_5.png" alt="Tendencia 5" width="40" /> |

El complemento ofrece dos widgets para mostrar las tendencias:

> - Rosée/Tendencia (Icono 40x40) (Widget predeterminado)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Rosée/Tendance 80x80 (Icône 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>

# Temperaturas percibidas

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

## Más información

- **¿El complemento utiliza API de terceros?**

> No, el complemento realiza el cálculo internamente en función de la temperatura, la humedad y la velocidad del viento

- **¿Qué es el enfriamiento eólico (o índice Windchill)?**

> El enfriamiento por el viento, también conocido a veces como «factor viento» o «windchill», se refiere a la sensación de frío que produce el viento, aunque la temperatura real del aire ambiente no baje.

- **¿Y el índice de calor o «humidex»?**

> El índice de calor (nombre original en inglés: Heat Index (HI) o humedad) es un índice desarrollado en Estados Unidos.
>
> Combina la temperatura del aire ambiente y la humedad relativa, en zonas a la sombra, para intentar determinar la percepción de la temperatura que experimenta el cuerpo humano, es decir, cuánto calor sentiría si la humedad relativa tuviera otro valor a la sombra.
>
> Este resultado también se conoce como la «temperatura percibida» o «temperatura aparente».
>
> Por ejemplo, cuando la temperatura es de 32 °C (o 90 °F) con un 70 % de humedad relativa:
>
> - El índice de calor es entonces de 41 °C (o 106 °F).
> - Esta temperatura del índice de calor tiene una humedad implícita (no especificada) del 20 %.
> - Es el valor de la humedad relativa para el que la fórmula del índice de calor indica que 41 °C se perciben como 41 °C.
> - Una temperatura del índice de calor de 32 °C tiene una humedad relativa implícita del 38 %.
>
> El índice de calor se basa en la capacidad del cuerpo humano para enfriar la piel mediante la producción de sudor.
>
> Esta se evapora en el aire, lo que requiere energía que se extrae del entorno y reduce la temperatura de la capa límite en contacto con la piel, lo que proporciona una sensación de frescor.
>
> A medida que aumenta la humedad relativa del aire, la evaporación se produce con mayor dificultad y provoca una sensación subjetiva de mayor calor. Este índice no debe confundirse con el factor «humidex» canadiense, que utiliza otra fórmula para cuantificar el mismo efecto.
