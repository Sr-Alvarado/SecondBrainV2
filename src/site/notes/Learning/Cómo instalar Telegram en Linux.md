---
{"dg-publish":true,"dg-path":"Cómo instalar Telegram en Linux.md","permalink":"/como-instalar-telegram-en-linux/","created":"2024-03-02T22:09","updated":"2024-03-02T22:09"}
---

Cuando queremos instalar Telegram el equipo de la app nos ofrece varias opciones, sin embargo no cuentan con un `.deb`, si eres linuxero de corazón no querrás instalar la versión [[snap\|snap]] y sabrás que [[flatpak\|flatpak]] suele dar problemas, entonces... Solo nos queda instalar desde los [[binarios\|binarios]], asi que allí vamos.

## Como instalar Telegram Desktop desde `.tar.xz`
Fuente original: [How to install Telegram on Linux Desktop in 2023 - Linux Shout](https://linux.how2shout.com/how-to-install-telegram-on-linux-desktop-in-2023/#Option_2_Use_the_official_Telegram_Desktop_PPA_for_Ubuntu_and_derivatives)
1. Descarga la ultima versión de Telegram desde la web oficial ejecutando este comando:
   ```shell
   wget "https://telegram.org/dl/desktop/linux" -O telegram.tar.xz
   ```
2. Extrae las carpetas de instalación[^1] con este comando:
   ```shell
   tar -xvf telegram.tar.xz
   ```
3. Mueve las carpetas extraídas al fichero `/opt/`[^2] para evitar borrarlas por error.
   ```shell
   sudo mv Telegram /opt/
   ```
4. Ejecuta la aplicación y crear un acceso directo al lanzador de aplicaciones.
   1. Accede a la nueva ubicación de Telegram
         ```shell
         cd /opt/Telegram/
         ```
   2. Ejecuta el binario
         ```shell
         ./Telegram
         ```
5. Se abrirá la aplicación, por el momento ciérrala.
6. Ahora abre el menú de aplicaciones y voalá, ya tienes Telegram instalado en Linux desde los binarios.

Eso es todo, espero que te este pequeño tutorial te haya ayudado.

[^1]: Al finalizar este paso técnicamente ya podrías ejecutar la aplicación, sin embargo al tener los ficheros base de la aplicación tan expuestos podrías borrarlos por error eliminando la aplicación.
[^2]: Esta es la carpeta donde Linux guarda aplicaciones opcionales de terceros.