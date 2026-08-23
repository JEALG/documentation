# Complemento Freebox_OS

<img src="{{site.baseurl}}/plugin-freebox_os/{{site.img}}/Freebox_OS_icon.png" class="pluginLogo" width="100" />

## Resolución de problemas

- **No me aparece el mensaje de autorización que se muestra en el Freebox**

  > Comprueba en la configuración del sistema operativo de la Freebox que la opción **Permitir nuevas solicitudes de asociación** esté marcada _(Configuración de la Freebox -> Gestión de accesos -> Pestaña «Parámetros»)_
  >
  > <p><img src="../images/freebox_association.png" alt="Asociación" width="500" /></p>

- **No veo el nivel de batería en el sensor de presencia de la Freebox ni en el mando a distancia**

  > esta información no se transmite a la Freebox, por lo que es imposible obtenerla en Jeedom.
  >
  > Por lo tanto, no están disponibles en la página de salud (aparece indicado «sector» o «N/A»).

- **No puedo activar la sirena de la alarma de la Freebox**

  > No es posible controlar directamente esta sirena
  > [Ver Bugtracker Freebox FS#30650](https://dev.Freebox.fr/bugs/task/30650)

- **Me aparece el mensaje «Versión de API desconocida»**

  > **Para que el complemento funcione, es necesario tener la Freebox en la versión 4.7 como mínimo**

  > - Una vez a la semana se ejecuta una comprobación automática de la versión de la API de Freebox.
  > - Se puede iniciar directamente desde la pantalla de emparejamiento
  > - Actualmente es obligatorio restablecer la clave API cada vez que se realiza una actualización
  >
  > <p><img src="../images/reset_api1.png" alt="Restablecer API Freebox" width="500" /></p>
  >
  > <p><img src="../images/reset_api2.png" alt="Restablecer API de Freebox" width="500" /></p>

- **Me aparece el mensaje «host desconocido, utiliza la dirección IP o maFreebox.Freebox.fr» y el demonio no funciona**

  - Tras la actualización de la Freebox a la versión 4.2.3
  > Free ha cambiado la dirección de la Freebox **_maFreebox.free.fr_**; esta ya no funciona, hay que sustituirla por **_maFreebox.Freebox.fr_**
  >
  > Consulta el apartado **Instalación y configuración**

- **Tengo el widget de dispositivos conectados, que ya no está disponible**

  > «El widget ha cambiado de nombre tras una actualización».
  >
  > Hay que **buscar equipos adicionales** para poder utilizar el nuevo widget

- **Me aparecen los siguientes mensajes: «Missing device_name» o «Tu Jeedom no tiene nombre, no es posible continuar» durante el emparejamiento**

  > **Tu Jeedom no tiene nombre**
  >
  > Es imprescindible que tu Jeedom tenga un nombre para poder continuar con el emparejamiento del complemento con tu Freebox.
  >
  > Ve a Ajustes -> Sistema -> Configuración -> pestaña General y asigna un nombre
  >
  > A continuación, vuelve a iniciar el proceso de autenticación sin olvidar restablecer la configuración.
  >
  > <p><img src="../images/nom_jeedom_1.png" alt="Falta el nombre del dispositivo" width="800" /></p>
  >
  > <p><img src="../images/nom_jeedom_2.png" alt="Nombre de Jeedom" width="800" /></p>

- **Error de CronDaily con nombres de dispositivos que incluyen iconos**

  > - Los nombres de los dispositivos no deben incluir iconos.

- **Los nuevos «Dispositivos conectados» y «Dispositivos conectados a la red Wi-Fi de invitados» no aparecen al actualizar el equipo**

  > - Los nuevos dispositivos no se añaden durante la actualización, sino únicamente con la tarea programada diaria.

- **No hay ningún mensaje en los registros en modo depuración**

  > - En cuanto a la parte de Tile, dado que la actualización se realiza varias veces por minuto, para evitar que se llenen los registros. No aparece ningún mensaje en los registros.
  >
  > Para obtener los registros de un dispositivo, hay que hacer clic en el botón «Actualizar» de dicho dispositivo.

- **Me aparece el mensaje «MÉTODO OBSOLETO» => POR FAVOR, CONSULTA LA DOCUMENTACIÓN**

  > Los comandos han cambiado en la sección de red, por lo que es necesario modificar el método para utilizar los comandos que se indican a continuación. *Consulta el apartado «Gestión de red»*
  >
  > Los siguientes comandos se eliminarán en la próxima actualización:
  >
  > - **«Añadir - Eliminar filtrado de Mac»** para los dispositivos *WIFI*
  > - **«Añadir o eliminar una IP fija»** para los dispositivos *Dispositivos conectados* y *Dispositivos conectados a la red Wi-Fi de invitados*
  > - **«Wake on LAN»** para los dispositivos *Dispositivos conectados* y *Dispositivos conectados a la red Wi-Fi de invitados*

- **¿A qué corresponden los distintos motores de tareas?**

  > - **RefreshToken**: Permite actualizar el acceso a la Freebox
  >
  > - **FreeboxPUT**: Permite realizar acciones en el Freebox
  >
  > - **FreeboxAPI**:
    > Permite probar y comprobar la última versión de la API de Freebox
    > Se realiza una comprobación una vez a la semana
  >
  > - **FreeboxGET**: Permite recuperar datos informativos relacionados con la domótica

- **El estado del reproductor no se actualiza**

  > Hay que comprobar que el tipo del comando «Estado» sea el subtipo **Otro**
  > <p><img src="../images/player.png" alt="Reproductor" width="800" /></p>
  
- **El estado del reproductor no está disponible**

  > Es imprescindible realizar un escaneo de los equipos estándar con el reproductor encendido

- **Los comandos «Dispositivo conectado seleccionado» y «Selección de dispositivo conectado» en el equipo «Gestión de red»**

  > Estos comandos se crearán automáticamente a través de los dispositivos *Dispositivos conectados* y/o *Dispositivos conectados a la red Wi-Fi de invitados*.

- **No se puede iniciar el demonio**

  > El demonio solo podrá iniciarse si la autenticación y los permisos son correctos. Esto se configura desde el menú «emparejamiento».

- **El registro de cambios indica: Atención: es necesario tener la Freebox servidor en la versión x.x.x para que el complemento funcione.**

 > Para que el complemento funcione, es necesario disponer de una versión mínima de firmware.
 > <p><img src="../images/firmware.png" alt="Firmware Freebox" width="800" /></p>
 > La versión mínima del firmware se indica en el registro de cambios, al principio y al inicio de esta documentación.
