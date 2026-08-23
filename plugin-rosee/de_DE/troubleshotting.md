# Plugin „Rosée – Givre – Trend“

<img src="{{site.baseurl}}/plugin-rosee/{{site.img}}/rosee_icon.png" class="pluginLogo" width="100" />

## Fehlerbehebung

- Mir liegen dazu keine Informationen vor

> Die für die verschiedenen Berechnungen erforderlichen Geräte müssen genau angegeben werden.<br/>
> Über die Suchfunktion für Geräte können Sie nach Geräten suchen.

- Der Gefrierpunkt beträgt 5 °C

> Die Temperatur liegt über 5 °C, daher wird der Vereisungspunkt nicht mehr berechnet und sein Wert auf 5 festgelegt.

- Die Berechnung des Trends erfolgt nicht

> Man muss 4 Stunden warten, um beim Anlegen des Geräts korrekte Ergebnisse zu erhalten.
> Das Gerät muss aktiviert sein, um zu funktionieren, und die Option „Identische Werte wiederholen“ muss auf „Ja“ gesetzt sein.

## Fehlermeldung

### Das Feld „Berechnung“ darf nicht leer sein

```
Le champ "Calcul" ne peut être vide
```

> Es muss überprüft werden, ob das Feld „Berechnung“ nicht leer ist oder den Wert „keine“ enthält<br/>

![Leerberechnung](../{{site.img}}/erreur_calcul_vide.png)

### Das Feld „Temperatur“ darf nicht leer sein

```
Le champ "Température" ne peut être vide
```

> Stellen Sie sicher, dass im Feld mit dem blauen Pfeil ein Gerät ausgewählt ist (siehe Abbildung unten)<br/>

### Das Feld „Relative Luftfeuchtigkeit“ darf nicht leer sein

```
Le champ "Humidité Relative" ne peut être vide
```

> Stellen Sie sicher, dass im Feld mit dem roten Pfeil ein Gerät ausgewählt ist (siehe Abbildung unten)<br/>

### Das Feld „Luftdruck“ darf nicht leer sein

```
Le champ "Pression Atmosphérique" ne peut être vide
```

> Stellen Sie sicher, dass im Feld mit dem orangefarbenen Pfeil ein Gerät ausgewählt ist (siehe Abbildung unten). Dieser Fehler tritt nur auf, wenn das Feld **Berechnungsart** den Wert **_Wettertrend_**<br/> hat.

![Leerberechnung](../{{site.img}}/erreur_champ_vide.png)

### Der Verlauf der Druckaufträge muss aktiviert sein

```
L'historique de la commande xxx doit être activé
```

> Der Bestellverlauf für Bestellung xx muss unbedingt aktiviert sein.
(siehe Abbildung unten)<br/>

![Geschichte](../{{site.img}}/pression1.png)
<br/>
![Geschichte](../{{site.img}}/pression2.png)

In bestimmten Fällen empfiehlt es sich außerdem, die Option „Identische Werte wiederholen“ zu aktivieren, um Fehler bei den Berechnungen zu vermeiden.
![Geschichte](../{{site.img}}/pression3.png)
