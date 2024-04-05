---
{"dg-publish":true,"dg-path":"Code/Trabajo local con Git.md","permalink":"/code/trabajo-local-con-git/","created":"2024-04-04T14:27","updated":"2024-04-04T19:03"}
---


> [!info]-
>> [!cite]+ **Fuentes y enlaces de interés:**
>> - [Curso de GIT y GITHUB desde CERO para PRINCIPIANTES - YouTube](https://youtube.com/watch?v=3GymExBkKjE)

Los pre-requisitos son,  tener [[Learning/Code/Git#^96012c\|instalado Git]] en una [[Learning/Code/Git Terminal/v - Versión de Git\|versión]] reciente, tener configurado el [[Learning/Code/Git Terminal/config user name - Configurar el usuario en Git\|usuario]] y el [[Learning/Code/Git Terminal/config user mail - Configurar el email en Git\|correo]]. Ya con estas configuraciones el flujo de trabajo sería:

## Flujo básico para proyectos simples
![Pasted image 20240404185732.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240404185732.png)
Este flujo de trabajo es recomendado para proyectos pequeños y simples, se usa solo la rama [[Learning/Wiki/Main\|principal]]. Si piensas llevar a producción tu proyecto debes seguir un flujo más avanzado

## Flujo con distintas ramas
![Pasted image 20240404185513.png|100%](/img/user/Engine/Attachments/Pasted%20image%2020240404185513.png)
Si tu proyecto se hace más grande debes ser más cuidadoso con las modificaciones, lo más recomendable es crear ramas alternas, una rama por cada característica adicional que quieras añadir. Una vez que estés seguro que la característica es estable puedes [[Learning/Code/Git Terminal/merge - Fusionar la rama actual con otra rama en Git\|mergearla]] a la rama principal. Puedes hacer tantas ramas como deses o necesites. 
