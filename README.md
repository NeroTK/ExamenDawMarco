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

1. Acceder a la máquina remota mediante SSH. Esto lo he realizado mediante el comando: ssh usuario@192.168.0.148
   ![ConectarSSH](https://github.com/NeroTK/ExamenDawMarco/blob/main/ConectarSSH.png)
2. Ir al escritorio de la maquina remota y crear un archivo de texto con el nombre especificado
   ![CrearArchivo](https://github.com/NeroTK/ExamenDawMarco/blob/main/CrearArchivo.png)
3. Escribir el resultado de whoami en el archivo de texto
   ![EscribirWhoami](https://github.com/NeroTK/ExamenDawMarco/blob/main/EscribirWhoami.png)
