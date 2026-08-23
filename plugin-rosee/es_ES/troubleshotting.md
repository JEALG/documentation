# Complemento «Rosée» - «Givre» - «Tendance»

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Resolución de problemas

- No tengo información al respecto

> Es necesario indicar claramente los equipos necesarios para los distintos cálculos.<br/>
> Se pueden buscar los dispositivos mediante el botón de búsqueda de dispositivos.

- El punto de congelación es igual a 5 °C

> La temperatura supera los 5 °C, por lo que ya no se calcula el punto de congelación y su valor se fija en 5.

- El cálculo de la tendencia no se realiza

> Hay que esperar 4 horas para obtener resultados correctos al crear el equipo.
> Para que el dispositivo funcione, debe tener activado el historial y la opción «Repetir valores idénticos» debe estar en «Sí».

## Mensaje de error

### El campo «Cálculo» no puede quedar vacío

```
Le champ "Calcul" ne peut être vide
```

> Hay que comprobar que el campo «cálculo» no esté vacío ni sea igual a «ninguno» <br/>

![Cálculo del volumen](../{{site.img}}/erreur_calcul_vide.png)

### El campo «Temperatura» no puede estar vacío

```
Le champ "Température" ne peut être vide
```

> Hay que comprobar que haya un dispositivo seleccionado en el campo con la flecha azul (véase la imagen siguiente)<br/>

### El campo «Humedad relativa» no puede estar vacío

```
Le champ "Humidité Relative" ne peut être vide
```

> Hay que comprobar que haya un dispositivo seleccionado en el campo con la flecha roja (véase la imagen siguiente)<br/>

### El campo «Presión atmosférica» no puede estar vacío

```
Le champ "Pression Atmosphérique" ne peut être vide
```

> Hay que comprobar que haya un equipo seleccionado en el campo con la flecha naranja (véase la imagen siguiente). Este error solo aparece si el campo **Tipo de cálculo** tiene el valor **_Tendencia meteorológica_**<br/>

![Cálculo del volumen](../{{site.img}}/erreur_champ_vide.png)

### El historial del comando «Presión» debe estar activado

```
L'historique de la commande xxx doit être activé
```

> El historial del pedido xx debe estar activado obligatoriamente.
(véase la imagen a continuación)<br/>

![Historia](../{{site.img}}/pression1.png)
<br/>
![Historia](../{{site.img}}/pression2.png)

En algunos casos, también es recomendable activar la opción «Repetir valores idénticos» para evitar que se produzca el error durante los cálculos.
![Historia](../{{site.img}}/pression3.png)
