---
{"dg-publish":true,"dg-path":"Code/Como instalar Telegram en Linux.md","permalink":"/code/como-instalar-telegram-en-linux/","created":"2024-03-02T22:09","updated":"2024-04-03T19:47"}
---

> [!info]-
>> [!cite]+ Fuentes y enlaces de interés 
>> - [How to install Telegram on Linux Desktop in 2023 - Linux Shout](https://linux.how2shout.com/how-to-install-telegram-on-linux-desktop-in-2023/#Option_2_Use_the_official_Telegram_Desktop_PPA_for_Ubuntu_and_derivatives)

Si deseas aprender a instalar Telegram desde su código fuente, los binarios del programa, este tutorial es para ti.

## Como instalar Telegram Desktop desde `.tar.xz`
Descarga la ultima versión de Telegram desde la web oficial ejecutando este comando:
```shell
wget "https://telegram.org/dl/desktop/linux" -O telegram.tar.xz
```

Extrae las carpetas de instalación[^1]:
```shell
tar -xvf telegram.tar.xz
```

Mueve las carpetas extraídas al fichero `/opt/`[^2] para evitar borrarlas por error:
```shell
sudo mv Telegram /opt/
```

Accede a la nueva ubicación de Telegram:
```shell
cd /opt/Telegram/
```

Ejecuta el binario:
```shell
./Telegram
```

Se abrirá la aplicación, por el momento ciérrala.

Ahora abre el menú de aplicaciones y voalá, ya tienes Telegram instalado en [[Learning/Wiki/Linux\|Linux]] desde los binarios.

Eso es todo, espero que te este pequeño tutorial te haya ayudado.

[^1]: Al finalizar este paso técnicamente ya podrías ejecutar Telegram, sin embargo al tener los ficheros base de la aplicación tan expuestos podrías borrarlos por error eliminando la aplicación.
[^2]: Esta es la carpeta donde [[Learning/Wiki/Linux\|Linux]] guarda aplicaciones opcionales de terceros.
[^3]: En realidad hay una versión .deb, ejecutando `sudo apt install telegram-desktop`, pero es muy antigua.