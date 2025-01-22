Configuración inicial

1. Preparación del sistema

Copia la carpeta raíz del sistema en cualquier directorio de tu computadora.

Asegúrate de que el archivo puerto.txt se encuentra en la carpeta raíz. Este archivo define el puerto de red que utilizará el sistema, y su valor por defecto es 5000. Puedes editarlo si necesitas usar un puerto diferente.

2. Iniciar el configurador

Ejecuta el archivo configurador. Es posible que requiera permisos de administrador, así que asegúrate de otorgarlos si el sistema lo solicita.

Una vez iniciado, el configurador mostrará la IP y el puerto que el sistema utilizará. Anota esta información, ya que será necesaria en los siguientes pasos.

3. Configuración de IP y puerto


Dirígete al archivo ip_config.txt, ubicado en la carpeta www/configuración.

Edita este archivo y asegúrate de ingresar la IP y el puerto proporcionados por el configurador en el paso anterior, en el formato:

[IP]:[PUERTO]
Por ejemplo: 192.168.1.100:5000.

4. Preparación del archivo CSV

Asegúrate de que el archivo Articulos.CSV se encuentra en el directorio www/.

Este archivo debe contener la información de los productos que serán utilizados por el sistema.


Uso del sistema

1. Ejecutar el configurador

Siempre debes tener el archivo configurador en ejecución para que el sistema funcione correctamente.

2. Acceder al sistema

Desde cualquier dispositivo conectado a la misma red, abre un navegador web y accede al sistema utilizando la IP y el puerto proporcionados por el configurador, en el formato:

http://[IP]:[PUERTO]
Por ejemplo: http://192.168.1.100:5000.

3. Configuración del tiempo de inactividad

Dentro de la carpeta www/configuración encontrarás un archivo llamado tiempo_config.txt.

En este archivo, puedes configurar el tiempo de espera antes de que se active el protector de pantalla, especificado en milisegundos.

El valor predeterminado es 5000 (5 segundos). Si deseas modificarlo, ingresa el tiempo deseado y guarda el archivo.

Notas importantes

El configurador debe estar en ejecución siempre para que el sistema de verificación funcione correctamente.

Puedes acceder al sistema desde cualquier dispositivo que esté conectado a la misma red.

Si cambias el puerto en el archivo puerto.txt, asegúrate de reiniciar el configurador para que los cambios surtan efecto.

Ejemplo de estructura de archivos

Carpeta raíz/
├── configurador
├── puerto.txt
└── www/
    ├── Articulos.CSV
    ├── configuración/
    │   ├── ip_config.txt
    │   └── tiempo_config.txt
    └── otros_archivos
