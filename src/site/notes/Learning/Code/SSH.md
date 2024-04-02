---
{"dg-publish":true,"dg-path":"Code/SSH.md","permalink":"/code/ssh/","created":"2024-03-30T22:57","updated":"2024-04-01T18:47"}
---


> [!info]-
>> [!cite]+ **Fuentes y enlaces de interés:**
>> - [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)
>> - [Conectar a GitHub con SSH - Documentación de GitHub](https://docs.github.com/es/authentication/connecting-to-github-with-ssh)
>> - [¿Qué es SSH? Significado de SSH en Linux](https://www.freecodecamp.org/espanol/news/que-es-ssh-significado-de-ssh-en-linux/)

## ¿Qué es SSH?
Es un protocolo criptográfico de comunicación en red segura basado [[clave privada\|clave privada]] y [[clave pública\|clave pública]]. 

### ¿Cómo funciona?
El proceso de comunicación entre el servidor y el usuario se hace de esta manera:
- El **cliente** inicia la conexión con el servidor, solicita un canal seguro. 
- El **servidor** genera 2 claves criptográficas, una pública que se envía al usuario y otra privada que guarda de forma segura en si mismo. 
- El **cliente** [[Learning/Code/Como generar una clave aleatoria en la terminal\|genera una clave aleatoria]] (clave de sesión) y la cifra usando la clave pública que le devolvió el servidor, y luego, envía la clave cifrada al servidor.
- El **servidor** descifra la clave usando su clave privada, y luego, envía un mensaje de éxito al usuario.

Desde este momento todos los datos transmitidos entre cliente-servidor son cifrados con la clave del usuario (clave de sesión).

## Uso
### Usar SSH para autentificarse en GitHub
[[Learning/Code/GitHub\|GitHub]] ya tiene en su documentación una explicación clara de como hacer esto por ello vamos a usarla:
- Si ya **tienes una clave SSH** en tu dispositivo puedes usarla para autentificar tu dispositivo en GitHub: [Comprobar tus claves SSH existentes - Documentación de GitHub](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys) 
- Si aún **no tienes una clave SSH** debes crearla: [Generación de una nueva clave SSH y adición al agente SSH - Documentación de GitHub](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) 
