# Complemento Tendance Baro

<img src="{{site.baseurl}}/plugin-tendance_baro/{{site.img}}/baro_icon.png" class="pluginLogo" width="100" />

## Descripción

Este complemento permite calcular la tendencia meteorológica prevista basándose en la evolución de la presión atmosférica de las últimas horas.

## Configuración

El complemento no tiene configuración general.
Hay que añadir un dispositivo para medir la presión atmosférica.

> Este dispositivo debe tener el historial activado

## Tendencias meteorológicas

> Fuentes:
>
> - <a href="http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf">http://www.freescale.com/files/sensors/doc/app_note/AN3914.pdf</a>
> - <a href="https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf">https://www.parallax.com/sites/default/files/downloads/29124-Altimeter-Application-Note-501.pdf</a>

El complemento calcula seis niveles de información

|  Nivel  | Tendencia | Imagen del widget |
| :------: | :--------------------------------- | :----------------------------------------------------------------: |
| <b>0</b> | Fuerte deterioro, inestable | <img src="../images/tendance_0.png" alt="Tendencia 0" width="40" /> |
| <b>1</b> | Deterioro, mal tiempo prolongado | <img src="../images/tendance_1.png" alt="Tendencia 1" width="40" /> |
| <b>2</b> | Deterioro lento, tiempo estable    | <img src="../images/tendance_2.png" alt="Tendencia 2" width="40" /> |
| <b>3</b> | Mejora lenta, tiempo estable   | <img src="../images/tendance_3.png" alt="Tendencia 3" width="40" /> |
| <b>4</b> | Mejora, buen tiempo duradero   | <img src="../images/tendance_4.png" alt="Tendencia 4" width="40" /> |
| <b>5</b> | Fuerte repunte, inestable | <img src="../images/tendance_5.png" alt="Tendencia 5" width="40" /> |

## El complemento ofrece dos widgets para mostrar las tendencias:

> - Baro/Tendencia (icono 40x40) (widget predeterminado)

<p><img src="../{{site.img}}/visu_tendance.png" width="200" alt="Visu Tendance 40x40" /></p>

> - Baro/Tendencia 80x80 (Icono 80x80)

<p><img src="../{{site.img}}/visu_tendance_80x80.png" width="200" alt="Visu Tendance 80x80" /></p>
