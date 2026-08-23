# Rosée - Givre - Trend Plug-in

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Troubleshooting

- I don't have any information on that

> Be sure to specify the equipment required for the various calculations.<br/>
> You can search for devices using the device search button.

- The freezing point is 5°C

> The temperature exceeds 5°C, so the frost point is no longer calculated and its value is set to 5.

- The trend is not calculated

> You must wait 4 hours to get accurate results when creating the device.
> The device must have "History" enabled to function and have "Repeat identical values" set to Yes.

## Error message

### The "Calculation" field cannot be left blank

```
Le champ "Calcul" ne peut être vide
```

> Make sure the "calculation" field is not empty or equal to "none"<br/>

![Empty Calculation](../{{site.img}}/erreur_calcul_vide.png)

### The "Temperature" field cannot be left blank

```
Le champ "Température" ne peut être vide
```

> Make sure that a device is selected in the field marked with the blue arrow (see image below)<br/>

### The "Relative Humidity" field cannot be left blank

```
Le champ "Humidité Relative" ne peut être vide
```

> Make sure a device is selected in the field marked with the red arrow (see image below)<br/>

### The "Atmospheric Pressure" field cannot be left blank

```
Le champ "Pression Atmosphérique" ne peut être vide
```

> Make sure a device is selected in the field with the orange arrow (see image below). This error appears only if the **Calculation Type** field has the value **_Weather Trend_**<BR/>

![Empty Calculation](../{{site.img}}/erreur_champ_vide.png)

### The "Pressure" command history must be enabled

```
L'historique de la commande xxx doit être activé
```

> The command history for command xx must be enabled.
(see image below)<br/>

![History](../{{site.img}}/pression1.png)
<br/>
![History](../{{site.img}}/pression2.png)

In some cases, it is also recommended to enable "Repeat identical values" to avoid errors during calculations
![History](../{{site.img}}/pression3.png)
