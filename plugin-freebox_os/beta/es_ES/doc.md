# Complemento Freebox_OS

<img src="{{site.baseurl}}/plugin-freebox_os/{{site.img}}/Freebox_OS_icon.png" class="pluginLogo" width="100" />


## Descripción

Este complemento permite recuperar la información de tu FreeboxOS (servidor Freebox Révolution, 4K, DELTA, POP o Ultra) e interactuar con él a través de widgets o escenarios que incorporan los comandos creados.

>
> **Para que el complemento funcione, es necesario disponer de la Freebox Serveur en la versión 4.12.1**

La información disponible de tu Freebox Servidor en Jeedom es la siguiente:

- **Información del sistema:**
  - Desconectar el wifi
  - Reiniciar tu Freebox
  - Velocidades de Internet
  - El estado de tu conexión
  - Gestión del filtrado de llamadas
- **Teléfono:** en las últimas 24 horas
  - Número de llamadas perdidas
  - El número de llamadas realizadas
  - El número de llamadas recibidas
  - Número de mensajes de voz
- **Disco duro:**
  - El espacio disponible en tus discos conectados al Freebox Servidor.
- **Dispositivos conectados a la LAN y a la red Wi-Fi de invitados:**
  - El estado de cada dispositivo DHCP
  - Posibilidad de utilizar el comando **_Wake on LAN_** únicamente mediante escenarios
- **Domótica (solo para el modelo DELTA):**
  - Recopila la información de la casa conectada

## Instalación y configuración

Una vez instalado y activado el complemento, no es necesario realizar ninguna configuración.

## Emparejamiento (autenticación)

Hay que ir a la página principal del complemento y hacer clic en

<p><img src="../images/appairage.png" alt="Ventana modal de emparejamiento" width="60" /></p>

A continuación, hay que seguir las distintas pantallas para confirmar el emparejamiento

<p><img src="../images/freebox_os_screenshot2.png" alt="Autenticación 1" width="300" /></p>

### Configuración

En la ventana que aparece a continuación, es posible modificar

- **IP Freebox**: Dirección de conexión de la Freebox _(por defecto: maFreebox.Freebox.fr)_
- **Nombre del dispositivo conectado**: El nombre del Jeedom (este campo está bloqueado)
- **Añadir automáticamente los dispositivos detectados en:**: Indicar la habitación por defecto
- Puedes hacer clic en el botón **Restablecer configuración** para recuperar los parámetros predeterminados.
  > - Recupera el **nombre de tu Jeedom** si ha cambiado desde el último emparejamiento
  > - Restablece los valores predeterminados para:
  >     - **Versión API de la Freebox**: v10
  >     - **IP Freebox**: maFreebox.Freebox.fr
  >     - Borra el resto de configuraciones del complemento

- No olvides hacer clic en **Guardar** después de realizar los cambios.

> Es imprescindible que tu Jeedom tenga un nombre para poder continuar con el emparejamiento del complemento con tu Freebox.

<p><img src="../images/freebox_os_screenshot3.png" alt="Autenticación 2" width="300" /></p>

### Autenticación

#### Firmware mínimo de la Freebox

 > Para que el complemento funcione, es necesario disponer de una versión mínima de firmware.
 > La versión mínima del firmware se indica en el registro de cambios, al principio y al inicio de esta documentación.

#### Autenticación

En la ventana que aparece a continuación se llevará a cabo el proceso de autenticación en el Freebox

- Haz clic en el botón **Iniciar autenticación**
- Sigue tanto las identificaciones que aparecen en esta pantalla como las de la Freebox

<p><img src="../images/freebox_os_screenshot4.png" alt="Autenticación 3" width="300" /></p>

### Verificación de derechos

En la ventana que aparece a continuación, el sistema comprobará los permisos asignados a la aplicación

- Consulta la sección «Derechos de acceso» (en esta documentación) para modificar los derechos en la Freebox.
- Una vez configurados los permisos, haz clic en el botón **Comprobación de permisos**.
  > Si los permisos son correctos, aparecerá el botón **Siguiente**
  > Los derechos obligatorios aparecen en negrita

<p><img src="../images/freebox_os_screenshot5.png" alt="Autenticación 4" width="300" /></p>

### Conectar los dispositivos Freebox con los dispositivos Jeedom

> Esta ventana solo aparece si la Freebox es un modelo DELTA
>
> Es posible activar o desactivar la tarea Cron «Actualización global de los mosaicos».
>
> <b>No olvides</b> hacer clic en «Guardar» para que se apliquen los cambios

<p><img src="../images/freebox_os_screenshot6.png" alt="Autenticación 4" width="300" /></p>

### Escanear

En la ventana que aparece a continuación, es posible iniciar el escaneo de los distintos dispositivos.

<p><img src="../images/freebox_os_screenshot7.png" alt="Autenticación 5" width="300" /></p>

### Autenticación completada

La autenticación se ha realizado correctamente.

<p><img src="../images/freebox_os_screenshot8.png" alt="Autenticación 6" width="300" /></p>

### Problema de autenticación resuelto

Si surge algún problema de autenticación, hay que proporcionar los registros del complemento en modo depuración
He aquí un ejemplo
```
000|[2024-10-11 18:53:49] INFO  ──────────▶︎ Étape : setting
0001|[2024-10-11 18:53:49] INFO  ───▶︎ IP : mafreebox.freebox.fr
0002|[2024-10-11 18:53:49] INFO  ───▶︎ Nom API : Plugin Freebox OS
0003|[2024-10-11 18:53:49] INFO  ───▶︎ Id API : plugin.freebox.jeedom
0004|[2024-10-11 18:53:49] INFO  ───▶︎ Nom de votre Jeedom : JAG Jeedom-VM2
0005|[2024-10-11 18:53:49] INFO  ───▶︎ Objet par défaut : 13
0006|[2024-10-11 18:53:49] INFO  ───▶︎ Version API Freebox : v12
0007|[2024-10-11 18:53:51] INFO  ──────────▶︎ Étape : authentification
0008|[2024-10-11 18:53:53] INFO  ──────────▶︎ Étape : rights
0009|[2024-10-11 18:53:57] DEBUG  OK  Close Session
0010|[2024-10-11 18:53:57] DEBUG  [Freebox Close Session] : {"uid":"","success":false,"msg":"Vous devez vous connecter pour accéder à cette fonction","result":{"password_salt":"","challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr"},"error_code":"invalid_session"}
0011|[2024-10-11 18:53:57] DEBUG  [Freebox Password] : {"success":true,"result":{"logged_in":false,"challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr","password_salt":"","password_set":true}}
0012|[2024-10-11 18:53:57] DEBUG  [get Freebox Open Session Data] : {"result":{"session_token":"eRDFtl35L8ENEND2UGlooFzLhAgmv8CGPbMLiegdyC2n4z3DDr4UEYY+zYMOhSkS","challenge":"sQn1Z4f3UT0u21ms1kogF\/pK+lnmuPTr","password_salt":"P","permissions":{"parental":true,"contacts":true,"explorer":true,"tv":true,"wdo":true,"downloader":true,"profile":true,"camera":true,"settings":true,"calls":true,"home":true,"pvr":true,"vm":true,"player":true},"password_set":true},"success":true}
0013|[2024-10-11 18:53:57] INFO  ───▶︎ Les droits sont OK
0014|[2024-10-11 18:53:58] INFO  ──────────▶︎ Étape : room
0015|[2024-10-11 18:53:58] INFO  ───▶︎ Cron Global Titles ACTIVATION : NOK
0016|[2024-10-11 18:53:58] INFO  ───▶︎ Compatibilité avec la partie domotique : NOK
0017|[2024-10-11 18:53:58] INFO  ──────────▶︎ Étape : scan
0018|[2024-10-11 18:53:59] INFO  ──────────▶︎ Étape : end
```

<p><img src="../images/debug_log.png" alt="Registro de activación en modo de depuración" width="300" /></p>


## Derechos de acceso

Para utilizar el complemento se necesitan algunos derechos de acceso adicionales, que **deben asignarse y modificarse** directamente desde el sistema operativo de la Freebox.

- Iniciar sesión en la interfaz de Freebox (http://maFreebox.Freebox.fr)
- Abrir la configuración de la Freebox

<p><img src="../images/freebox_para.png" alt="Configuración de la Freebox" width="100" /></p>

- Acceder a la gestión de accesos de la Freebox _(esta configuración se encuentra en el modo avanzado)_

<p><img src="../images/freebox_gestion_acces_1.png" alt="Configuración de gestión de accesos de la Freebox" width="600" /></p>

- Haz clic en la pestaña **Aplicaciones**
- En la lista, selecciona la aplicación indicada durante la instalación del complemento _(por defecto: Complemento Freebox OS)_

<p><img src="../images/freebox_gestion_acces_2.png" alt="Configuración de la gestión de accesos del Freebox" width="500" /></p>

- **Conceder todos los derechos de acceso**

<p><img src="../images/modification_droit.png" alt="Modificación de los derechos de acceso específicos" width="500" /></p>

# Equipos estándar

Haz clic en el botón **_Escanear equipos estándar_**; el complemento creará los distintos equipos estándar de la Freebox.

<p><img src="../images/recherche_systeme.png" alt="Búsqueda de equipos del sistema" width="60" /></p>

Se van a crear los siguientes dispositivos y controles:

- **Pantalla LCD**
  - Ajuste de la luminosidad
  - Ajuste de la orientación del texto
  - Ocultar la clave de la red Wi-Fi
  - Gestión de las tiras luminosas (si el router es compatible)
  - Apagar el LED (si el router es compatible)
- **Air Média**
  - Selección del reproductor actual
  - AirMedia Start / Stop
- **Dispositivos conectados** y **Dispositivos conectados a la red Wi-Fi para invitados**
  - Conjunto de dispositivos conectados a la Freebox
  - Posibilidad de utilizar el comando **_Wake on LAN_** (solo mediante escenarios)
- **Disco duro**
  - Espacio ocupado en el disco
  - Temperatura
  - Tipo de RAID (solo para Freebox compatibles)
- **Velocidades de Freebox**
  - Freebox: velocidad de descarga, velocidad de subida, ancho de banda de subida, ancho de banda de bajada
  - Freebox Media
  - Estado de Freebox
  - Tipo de conexión
  - Estado de la conexión
  - IP
  - Respuesta al ping
- **Reproductor**
  - Mac
  - Tipo
  - Modelo
  - Versión
  - API disponible
  - Disponible en la red
  - Estado (encendido o apagado)
    > El comando solo se crea si el reproductor devuelve su estado y tiene un ID.
    > **Es imprescindible que el reproductor esté encendido y no se encuentre en modo de suspensión prolongada (Révolution) durante la búsqueda**
    > Los reproductores mini4K/POP están disponibles, pero no informan de su estado
- **Compartir archivos entre Windows y Mac**
  - Activar/desactivar el uso compartido de archivos en Mac, Windows y FTP
  - Activar/Desactivar el uso compartido de impresoras (disponible solo si SMBv2 no está activo)
- **Sistema**
  - Actualización
  - Reinicio
  - Versión del firmware de Freebox
  - Mac
  - IP v4/v6
  - Velocidad del ventilador
  - Temperaturas _(temp sw, temp cpub, temp cpum)_
  - Activa desde
  - nombre de la placa
  - en serie
  - 4G si la tarjeta está insertada en la Freebox
- **Llamadas telefónicas** en las últimas 24 horas
  - Número de llamadas perdidas / recibidas / realizadas
  - Lista de llamadas perdidas / recibidas / realizadas
  - Número de mensajes de voz
  - Lista de mensajes de voz leídos y nuevos
- **Descargas**
  - Número de tareas
  - Número de tareas activas, en extracción, en reparación, en verificación, en espera, con error, detenidas, finalizadas, de fuentes RSS y de fuentes RSS sin leer
  - Descarga en curso
  - Velocidad de recepción y transmisión
  - Inicio, Parada
  - Modo de descarga
  - Estado de la planificación
  - Estado de la sesión
- **VM** (solo para Freebox compatibles)
  - Estado
  - Acciones posibles: Detener, Reiniciar, Iniciar
  - Información: número de CPU, dirección MAC, memoria, puerto USB, pantalla virtual, tipo de disco
- **Wi-Fi**
  - Estado de la red wifi
  - Wi-Fi activado/desactivado
  - Gestión del filtrado de llamadas
  - Estado de la planificación
  - Sesión WPS activada/desactivada
  - Lista negra de Mac
  - Lista blanca de Mac
  - Estado de la tarjeta wifi

## Control parental

Haz clic en el botón **_Escanear control parental_**; el complemento creará los distintos dispositivos del sistema de la Freebox.

> Estos controles se han implementado con la versión 4.2 de la Freebox.

<p><img src="../images/recherche_parental.png" alt="Búsqueda de controles parentales" width="60" /></p>

- Se van a crear los siguientes dispositivos y controles:
  
  > - Estado
  > - Bloquear
  > - Autorizar
  > - Bloquear 30 min/1 h/2 h

## Características específicas de los adaptadores domésticos (solo Freebox Delta), dispositivos conectados, disco duro y sistema

Estos cuatro dispositivos están vacíos por defecto al crearlos, salvo el sistema, que incluye la información común a todas las Freebox.

Abre cada dispositivo y haz clic en el botón «Buscar»

> El complemento buscará y creará los distintos comandos asociados

<p><img src="../images/recherche_commandes.png" alt="Búsqueda de equipos específicos" width="800" /></p>

> Una tarea programada diaria permite buscar automáticamente los nuevos dispositivos

## Gestión de redes

Este equipo permite:

> - Asignar una dirección IP fija
> - Gestionar el filtrado de direcciones MAC
> - Función Wake on LAN
> - Cambiar el tipo de dispositivo

### Asignar una dirección IP

<p><img src="../images/modif__equip_ip_fixe.png" alt="Modificación de la IP" width="800" /></p>

Es necesario rellenar los siguientes campos

- Seleccionar el dispositivo conectado
- Seleccionar y modificar el dispositivo con el siguiente valor

  > - **Añadir una dirección IP fija**
  > - **Eliminar IP fija**
  > - **Cambiar la dirección IP del dispositivo**

También se puede hacer con el comando
   > - **Cambiar el tipo de dispositivo / IP**

- Selección de IP: Indica la dirección IP del dispositivo
- Selección del nombre del dispositivo: Indica el nombre del dispositivo

  > Si el nombre está vacío, el complemento recuperará el nombre del dispositivo indicado en la Freebox

- Comentarios: permite introducir un comentario (Opcional)

### Cambiar el tipo de dispositivo

<p><img src="../images/modif__equip_type.png" alt="Modificación de los equipos" width="800" /></p>

Es necesario rellenar los siguientes campos

- Seleccionar el dispositivo conectado
- Seleccionar y modificar el dispositivo con el siguiente valor

  > - **Cambiar el tipo de dispositivo / IP**

- Selección del tipo de dispositivo: Selecciona el tipo de dispositivo

  > Si el nombre está vacío, el complemento recuperará el nombre del dispositivo indicado en la Freebox
  
- Comentarios: permite introducir un comentario
- Modificar el dispositivo: permite enviar la modificación a la Freebox

### Gestionar el filtrado de direcciones MAC (Wi-Fi)

<p><img src="../images/modif__equip_filtrage.png" alt="Modificación de los equipos" width="800" /></p>

Esto se puede hacer mediante los controles de los dispositivos conectados o con wifi.
Es necesario rellenar los siguientes campos

- Seleccionar el dispositivo conectado
- Seleccionar y modificar el dispositivo con el siguiente valor

  > - **Añadir/Modificar lista negra**
  > - **Añadir/Modificar lista blanca**
  > - **Eliminar lista negra/blanca**

- Comentarios: permite introducir un comentario o una contraseña
- Modificar el dispositivo: permite enviar la modificación a la Freebox

### Función Wake on LAN

<p><img src="../images/modif__equip_wol.png" alt="Modificación de los equipos" width="800" /></p>

- Seleccionar el dispositivo conectado
- Seleccionar y modificar el dispositivo con el siguiente valor

  > - **Wake on LAN**

- Comentarios: permite introducir una contraseña
- Modificar el dispositivo: permite enviar la modificación a la Freebox

Esta gestión se realiza a través de la interfaz desde el widget de dispositivos conectados o desde un escenario.

## Freebox Delta

> La Freebox Delta ofrece un paquete de seguridad y permite conectarse a determinados dispositivos.

Haz clic en el botón **_Scan Tiles_**; se crearán los dispositivos y los controles de los distintos dispositivos conectados.

<p><img src="../images/recherche_tiles.png" alt="Búsqueda de equipos específicos de Freebox Delta" width="60" /></p>

### Estado de la alarma

> El complemento muestra el estado de la alarma mediante el comando «Estado de la alarma».

![Estado de la alarma](../images/alarme_statut.png)
Los valores posibles son:

> **inactivo** = Alarma desactivada
> **alarm_1_arming** = La alarma principal está activada; se trata de una cuenta atrás en la que solo los sensores que no se encuentran en la zona pueden activar la alerta
> **alarm_2_arming** = La alarma parcial está activada; se trata de una cuenta atrás en la que solo los sensores que no se encuentran en la zona pueden activar la alerta
> **alarm_1_armed** = Alarma general activada
> **alarm_2_armed** = Alarma parcial activada
> **alarm1_alert_timer** = La alarma principal se ha activado mediante un sensor en la zona horaria y la sirena sonará tras una cuenta atrás
> **alarm2_alert_timer** = La alarma nocturna se ha activado mediante un sensor en la zona horaria y la sirena sonará tras una cuenta atrás
> **alerta** = Suena la sirena

> El sistema de alarma es compatible con Homebridge y la aplicación móvil: no es necesario realizar ninguna configuración.
> Para facilitar la integración, se han añadido comandos de información que permiten interactuar con el complemento «Alarma».
>
> - **Activo** = Información binaria (1 = Alarma activada)
> - **Estado** = Información binaria (1 = Sirena activa)

<p><img src="../images/alarme_dashboard.png" alt="Estado de la alarma" width="250" /></p>

### Estado del mando a distancia

> El complemento registra el historial del mando a distancia y muestra la última acción realizada con él.

- Los valores posibles son:
  > **null** o **0** = Sin estado
  > **1** = Alarma principal
  > **2** = Desactivación
  > **3** = Alarma secundaria

### Las cámaras

> Las cámaras se crean automáticamente si está instalado el complemento de cámara

## Tiempo de actualización (Cron) de los equipos

- Es posible modificar la configuración de Cron para la actualización de cada dispositivo; por defecto:

  > Home Adapter, FREEBOX: mando a distancia (alarma), control parental y «Mis dispositivos», excepto el disco duro = **Cron se configurará a 5 minutos**
  >
  > Disco duro = **Cron se configurará a la 1**

- Este Cron permite actualizar los distintos comandos de tipo informativo; el equipo se actualiza automáticamente cuando se ejecuta un comando.
  > Las órdenes de acción no se ven afectadas por este Cron.
  >
  > Cuanto más corto sea el tiempo, mayor será la carga sobre la CPU de la Freebox.

- Desde la versión 20210507 del complemento, para la **sección de domótica**
  > Por defecto, hay una tarea Cron de actualización global activada
  >
  > <p><img src="../images/cron_tiles.png" alt="Tiempo de actualización" width="800" /></p>
  >
  > Si esta opción está desactivada, el **Cron se configurará en 1 minuto**

## Los tiles

*No todos los dispositivos están necesariamente integrados en el sistema, dada la evolución de la Freebox*S

- Para poder integrar los nuevos sistemas, es necesario:

  > Poner el complemento en modo de depuración
  > Reiniciar el demonio
  > Crear **_Debug Tiles_**

<p><img src="../images/debug.png" alt="Mosaicos de depuración" width="60" /></p>

Abre un tema (si aún no hay ninguno que trate esta consulta) en la comunidad y facilita la siguiente información:

- Hacer una captura de pantalla del equipo

<p><img src="../images/tiles1.png" alt="Equipamiento tiles 1" width="800" /></p>

- Hacer una captura de pantalla de los controles del equipo

<p><img src="../images/tiles2.png" alt="Equipamiento tiles 2" width="800" /></p>

- Proporciona los registros en formato de texto y no una captura de pantalla
  > [Ver el apartado **11**. Formatear correctamente](https://community.jeedom.com/t/comment-nous-aider-a-vous-aider-ou-comment-poser-une-bonne-question/34932)

```
    [2020-08-24 07:37:41][DEBUG] : ┌───────── Commande trouvée pour l'équipement FREEBOX : FREEBOX - Eclairage Canapé -- Pièce : Salon (Node ID 9)
[2020-08-24 07:37:41][DEBUG] : │ Label : Enclenché -- Name : switch_state
[2020-08-24 07:37:41][DEBUG] : │ Type (eq) : light -- Action (eq): intensity_picker
[2020-08-24 07:37:41][DEBUG] : │ Index : 0 -- Value Type : bool -- Access : rw
[2020-08-24 07:37:41][DEBUG] : │ Valeur actuelle :
[2020-08-24 07:37:41][DEBUG] : │ Range : ----- -- Range color : -
[2020-08-24 07:37:41][DEBUG] : │ Name: Etat -- Type : info -- LogicalID : 0 -- Template Widget / Ligne : core::light/0-- Type de générique : LIGHT_STATE -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : │ No Repeat pour l'info avec le nom : Etat
[2020-08-24 07:37:41][DEBUG] : │ Name: On -- Type : action -- LogicalID : PB_On -- Template Widget / Ligne : core::light/1-- Type de générique : LIGHT_ON -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : │ Name: Off -- Type : action -- LogicalID : PB_Off -- Template Widget / Ligne : core::light/0-- Type de générique : LIGHT_OFF -- Inverser : 0 -- Icône :  -- Min/Max : default/default
[2020-08-24 07:37:41][DEBUG] : └─────────
[2020-08-24 07:37:41][DEBUG] : ┌───────── Commande trouvée pour l'équipement FREEBOX : FREEBOX - Eclairage Canapé -- Pièce : Salon (Node ID 9)
[2020-08-24 07:37:41][DEBUG] : │ Label : Luminosité -- Name : luminosity
[2020-08-24 07:37:41][DEBUG] : │ Type (eq) : light -- Action (eq): intensity_picker
[2020-08-24 07:37:41][DEBUG] : │ Index : 2 -- Value Type : int -- Access : rw
[2020-08-24 07:37:41][DEBUG] : │ Valeur actuelle : 254
[2020-08-24 07:37:41][DEBUG] : │ Range : ----- -- Range color : -
[2020-08-24 07:37:41][DEBUG] : │ Name: Etat Luminosité -- Type : info -- LogicalID : 2 -- Template Widget / Ligne : /0-- Type de générique : LIGHT_COLOR -- Inverser : 0 -- Icône :  -- Min/Max : 0/255
[2020-08-24 07:37:41][DEBUG] : │ No Repeat pour l'info avec le nom : Etat Luminosité
[2020-08-24 07:37:41][DEBUG] : │ Name: Luminosité -- Type : action -- LogicalID : 2 -- Template Widget / Ligne : default/0-- Type de générique : LIGHT_SET_COLOR -- Inverser : 0 -- Icône :  -- Min/Max : 0/255
[2020-08-24 07:37:41][DEBUG] : └─────────
```
