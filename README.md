# ExamenDawMarco
## Introducción
En este archivo MarkDown, documentaré paso a paso como he realizado los ejercicios 2 y 3 del examen de DAW, incluyendo capturas del proceso. El ejercicio 2 és de SSH, y en él tendré que acceder a una máquina remota para crear un archivo con mi nombre, que contenga el nombre de usuario de mi máquina, y concatenar el nombre de todos los conectados a la máquina remota. Por otro lado, el ejercicio 3 trata de crear un VirtualHost, en el que crearé un html con mi nombre, y lo ejecutare en el navegador mediante apache.

## Ejercicio 2: SSH
Para este ejercicio, teníamos que seguir el siguiente enunciado:
>Documenta todos los pasos realizados en un archivo MarkDown. Accede a esta máquina remota mediante ssh: **(Captura de pantalla con la ip 192.168.0.148)**
>
>Deberás ir al escritorio y crear un archivo de texto que contenga como nombre de archivo, tu nombre propio y apellido sin espacios y con extensión txt (por ejemplo ArnoldSchwarzenegger.txt) escribe en su interior el resultado de whoami.
Después, mediante otro comando, concatena al final del archivo el resultado del comando necesario para saber quién está conectado a la máquina mediante ssh.

Para poder realizar lo que pide el enunciado, he seguido los siguientes pasos:

1. Acceder a la máquina remota mediante SSH  
   ![ConectarSSH](https://github.com/NeroTK/ExamenDawMarco/blob/main/ConectarSSH.png)
2. Ir al escritorio de la maquina remota y crear un archivo de texto con el nombre especificado  
   ![CrearArchivo](https://github.com/NeroTK/ExamenDawMarco/blob/main/CrearArchivo.png)
3. Escribir el resultado de whoami en el archivo de texto  
   ![EscribirWhoami](https://github.com/NeroTK/ExamenDawMarco/blob/main/EscribirWhoami.png)
4. Concatenar información sobre quién está conectado mediante SSH  
   ![ConcatenarConectados](https://github.com/NeroTK/ExamenDawMarco/blob/main/ConcatenarConectados.png)
5. Verificar el contenido del archivo  
   ![ComprobarResultado](https://github.com/NeroTK/ExamenDawMarco/blob/main/ComprobarResultado.png)

## Ejercicio 3: VirtualHost
Para este segundo ejercicio, teníamos que seguir el siguiente enunciado:
>Documenta todos los pasos realizados en un archivo MarkDown. Crea en tu máquina un virtualhost donde escribiendo _“daw.ejercicio3.com”_ nos envíe a una web local que simplemente contenga tu nombre.

Para crear el VirtualHost y acceder a la web local, deberemos hacer lo siguiente:

1. Abrir el archivo de configuración de Apache con el editor nano  
   ![AbrirConfigApache](https://github.com/NeroTK/ExamenDawMarco/blob/main/AbrirConfigApache.png)
2. Agregar las siguientes líneas al archivo para configurar el VirtualHost  
   ![ConfiguracionVirtualHost](https://github.com/NeroTK/ExamenDawMarco/blob/main/ConfiguracionVirtualhost.png)
3. Crear el directorio **/var/www/daw_ejercicio3** y crear el **index.html**  
   ![CrearDirectorioYIndex](https://github.com/NeroTK/ExamenDawMarco/blob/main/CrearDirectorioyIndex.png)
4. Habilitar el nuevo sitio y reiniciar Apache  
   ![HabilitarSitio](https://github.com/NeroTK/ExamenDawMarco/blob/main/HabilitarSitio.png)
5. Agregar la linea **127.0.0.1   daw.ejercicio3.com** en /etc/hosts mediante el editor nano para apuntarlo en la máquina local  
   ![AñadirDireccionHosts](https://github.com/NeroTK/ExamenDawMarco/blob/main/A%C3%B1adirDireccionHosts.png)
6. Comprobar que funciona ingresando en el navegador la dirección: **daw.ejercicio3.com**
   ![ComprobarFuncionamiento](https://github.com/NeroTK/ExamenDawMarco/blob/main/ComprobarFuncionamiento.png)
