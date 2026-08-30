# Complemento «Rosée» - «Givre» - «Tendance»

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Información sobre el historial de cambios

### Importante

> **_Recordatorio_**: si no hay información sobre la actualización, es porque esta se refiere únicamente a la actualización de la documentación, a traducciones o a correcciones de errores menores.

## 2026

### 30/08/2026

- Traslado de la documentación beta y la traducción

### 06/03/2026

- Mejoras y actualización del complemento

## 2025

### 05/05/2025

- Se ha añadido el comando «Presión de vapor real» en Pa
_ Corrección de la unidad
- Se ha añadido el comando «proporción de mezcla» en g/kg: https://fr.m.wikipedia.org/wiki/Rapport_de_mélange


### 25/01/2025

- Actualización del enlace a la documentación

### 15-16/01/2025

- Incorporación de un controlador para la velocidad del viento


### 14/01/2025

- Corrección del cálculo de la temperatura percibida: https://community.jeedom.com/t/erreur-calcul-de-la-temperature-ressentie/136577

## 2024

### 30/12/2024

- Mejora del registro + traducción

### 28/12/2024

- Mejoras en el registro

### 01/11/2024

- Errores tipográficos

### 25/09/2024

- Corrección de un error en setConfiguration al crear comandos

### 22/09/2024

- Tendencia: si no hay datos en el historial, los datos de tendencia y la tendencia numérica no se actualizan
- Traducción  (Gracias, @Mips)

### 14/09/2024

- Traducción (Gracias, @Mips)
- corrección de PHP 8

### 21/08/2024

- Traducción
- Mejoras y actualizaciones en los controles
- Cambio del «logicalId» para el comando de escarcha (escarcha => frost_point)
- Cambio del «logicalId» para el comando «Humedad relativa» (humidityabs => humidityabs_m3)
- Tendencia: no se realiza el cálculo si el historial es nulo
- Errores tipográficos en CRON
- Mejoras en Log core 4.4

### 28/05/2024

- Corrección de valor nulo

### 26/05/2024

- Control del valor de parámetros específicos: interrupción de los cálculos si no hay ningún valor
- Mejora de los registros

### 04/02/2024

- Eliminación del enlace a la comunidad tras el cambio al núcleo 4.4
- Mejora de la visualización debajo de la tabla

### 14/01/2024

- Mejoras para Core V4.4

## 2023

### 08/10/2023

- Mejora de la información para la comunidad en Core 4.4
- Errores tipográficos

### 02/06/2023

- Actualización de información sobre el mercado

### 02/04/2023

- Corrección para Core 4.4
- La versión mini Core del complemento es la 4.2

### 20230327

- Errores tipográficos

## 2022

### Versión 20220212

- Pantalla Core v4.2
- Función Core v4.3
- El método js jeedom.eqLogic.builSelectCmd se ha renombrado correctamente: jeedom.eqLogic.buildSelectCmd.

## 2021

### Versión 20211101

- Añadir información JSON
- Se ha añadido información sobre la presión y se han corregido los comandos de creación
- Corrección en la creación de comandos de tendencia

### Versión 20211023

- Actualización tras el cambio al núcleo v4.2

### Versión 20210728

- Mejoras para Core v4.2

### Versión 20210510

- Añadir información al registro

### Versión 20210226

- Corrección de la temperatura percibida

### Versión 20210213

- Visualización de la tabla Core v4.2 (beta)
- Corrección del objeto principal
- Mejora general de la visualización

## 2020

### Versión 20201208

- Corrección del error en el cálculo del Humidex
- Corrección de diversos errores

### Versión 20201207

- Corrección de un error en la creación de comandos
- Corrección del error de «Mín.» y «Máx.» en los controles numéricos
- Se ha añadido el cálculo de la temperatura percibida para el invierno https://community.jeedom.com/t/temperature-ressentie/44377/2

### Versión 20201129

- Mejora de la visualización, incorporación de información emergente en los controles
- Mejoras y actualizaciones en los controles

### Versión 20201105

- Corrección de la visualización de los valores numéricos para los umbrales y el desplazamientohttps://community.jeedom.com/t/pas-dalerte-givre/41213/8

### Versión 20201031

- Mejora de la lista de objetos principales

### Versión 20201027

- Mejora visual en el panel de control

### Versión 20201026

- Mejora en la creación de pedidos
- Mejoras y actualizaciones en los controles
- Modificación de la visualización de los controles
- Se ha añadido el reinicio de la búsqueda de BP
- Clean Log + código
- Corrección del error «Rosee \_eqNameID» (error de prueba)
- Corrección de un error que provocaba la eliminación del comando «Refresh»
- Aviso de corrección de PHP
- Corrección: variable no definida
- Mejora si hay problemas históricos de presión
- Corrección de un error en la creación de comandos

### Versión 20200525

- Corrección de un error: recreación de los comandos
- Limpieza final tras el traslado de la documentación
- Mejora del código (gestión de la visualización de parámetros según el modo de cálculo)

### Versión 20200512

- Traslado de documentación
- Corrección de un error en el registro individual de cada dispositivo
- Registro de los dispositivos tras cada actualización
- Modificación del widget para la tendencia

### Versión 20200430

- Corrección: se ha añadido el widget Core por defecto en los nuevos dispositivos

### Versión 20200418

- Se ha añadido el cálculo «Tendencia meteorológica»
- Limpieza del registro
- Corrección de errores
- Correcciones de errores en la selección de equipamiento obligatorio
- Añadir tarea programada cada 10/15 horas
- Sustitución de Cron5 por Cron30 (los cálculos se realizarán, por defecto, cada 30 minutos)
  > **Nota: No olvides comprobar que Cron 30 esté activo; de lo contrario, tendrás que activarlo**
- Se ha añadido el widget Core para los controles (solo para los nuevos dispositivos)
- Incorporación de un widget para las tendencias (solo para Core V4 y los nuevos equipos)

### Versión 20200409

- Separación de cálculos
- Limpieza de la información de los registros
- Se ha añadido un botón para recrear los comandos
- Solución del error: la lista desplegable de opciones no se calcula correctamente
- No es necesario ocultar los parámetros según el método de cálculo
- Modificación en la creación de pedidos: ahora se tiene en cuenta el método de cálculo
- Eliminación de algunos cálculos intermedios
- Asignación de los valores mínimo y máximo al «mensaje numérico»

> Nota: No olvides hacer una copia de seguridad de cada dispositivo

### Versión 20200226

- El punto de escarcha es igual a 5 si la temperatura supera los 5 °
- Posibilidad de seleccionar solo una parte del cálculo (rocío y escarcha, humedad absoluta, escarcha, punto de rocío)
- Añadir un desplazamiento de temperatura (valor por defecto: 0)

### Versión 20200210

- El punto de escarcha es igual a la temperatura cuando esta es superior a 10 °C

### Versión 20200209

> _Nota: Cambio de autor del complemento, gracias @claude.metzger_

- Incorporación de un registro adicional en modo DEBUG
- Limpieza del código
- Nuevo cálculo para la gestión de la alerta de heladas
- Se ha añadido un mensaje para el tipo de escarcha, así como un valor numérico según el código <a href="https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue/">https://pon.fr/dzvents-alerte-givre-et-calcul-humidite-absolue</a>
  > - CAS N.º 0: Mensaje = _Sin riesgo de escarcha_, Alerta de escarcha = _0_, Mensaje numérico = _0_
  > - CASO N.º 1: Mensaje = _Es poco probable que se forme escarcha a pesar de la temperatura_, Alerta de escarcha = _1_, Mensaje numérico = _1_
  > - CASO N.º 2: Mensaje = _Riesgo de escarcha_, Alerta de escarcha = _1_, Mensaje numérico = _2_
  > - CASO N.º 3: Mensaje = _Hielo, Presencia de hielo_, Alerta de hielo = _1_, Mensaje numérico = _3_
- Cambio del logotipo del complemento. Gracias, @mich0111
- Corrección del tipo de créditos
- Posibilidad de registrar el equipo sin rellenar los campos obligatorios si el equipo no está activo
- Modificación de la visualización de los controles
  > - Se ha añadido la posibilidad de invertir los comandos binarios
  > - Eliminación del historial de mensajes de pedidos
- Se añaden los nuevos comandos de forma automática sin necesidad de volver a crearlos (gracias a Kiboost y a Mips)
- Modificación del tipo de datos para los umbrales => Solo numérico
- Se ha añadido un umbral de humedad absoluta para el cálculo de la alerta de escarcha
- No se calculan los datos de heladas si la temperatura es superior a 10 °C

  > _Nota: Es obligatorio guardar cada dispositivo para poder disponer de los nuevos comandos_


## <2020

### Versión 3.3.2

- Incorporación de un registro adicional en modo DEBUG
- Eliminación de la visibilidad para el cálculo del punto de rocío y del punto de escarcha

### Versión 3.3.1

- Corrección de la documentación

### Versión 3.3

- Corrección de errores

### Versión 3.2

- Incorporación de un Cron 30 (gracias a kiboost)
- Mejora de la visualización para Core V4 (gracias a kiboost)
- Posibilidad de cambiar el nombre de los comandos (gracias a kiboost)
- Corrección de los historiales (gracias a kiboost)
- Comando «Refresh» (en el mosaico, escenario, etc.) (Gracias a kiboost)
- Mejora de los registros
- Corrección típica de Generic
- Corrección de un error: los datos ya no se actualizan si el dispositivo está desactivado
- Las alertas se muestran de forma predeterminada (ya no se ocultan si el valor de la alerta es 0).
- Limpieza de carpetas (Gracias a kiboost)
- Actualización de la documentación

> _Nota: Se recomienda desinstalar el complemento y volver a instalarlo_

### Versión 3.1

- La búsqueda de los comandos para la actualización ya no se realiza mediante getConfiguration('data'), sino mediante su logicalId. Los comandos pierden sus datos de configuración. (gracias a jpty)

### Versión 3.0

- Compatibilidad con PHP 7.3
- Migración a Font Awesome 5
- Migración de la visualización al formato Core V4

### Versión 2.1

- Corrección de fallos en la visualización del punto de rocío y la formación de escarcha

### Versión 2.0

- Actualización para compatibilidad con Jeedom V3

### Versión 1.5.2

- Corrección de un error en rosee.class.php en la llamada a la función cron15() (gracias a mika-nt28 y Mika)

### Versión 1.5.1

- Se ha corregido un error en el cálculo del umbral de alerta de rocío.

### Versión 1.5

- Gestión de alertas de rocío y escarcha mediante cambio de estado (gracias, Toregreb)

### Versión 1.4

- Umbral de alerta del punto de rocío configurable en «Información». Valor por defecto: 2 °C

### Versión 1.3.1

- Ajuste del umbral de alerta del punto de rocío y del punto de escarcha a 2 °C (depresión del punto de rocío)

### Versión 1.3

- Incorporación de una alerta de punto de rocío y una alerta de punto de escarcha

### Versión 1.2

- Selección de la temperatura y la humedad (posible mediante un botón de búsqueda) (gracias, Lunarok)

### Versión 1.1

- Incorporación del punto de escarcha

### Versión 1.0

- Creación del complemento
