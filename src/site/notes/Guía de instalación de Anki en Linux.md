---
{"dg-publish":true,"permalink":"/guia-de-instalacion-de-anki-en-linux/","created":"2024-01-25T19:06","updated":"2024-02-02T17:58"}
---

## Instalación
**Fuente:** [Install & Upgrade - Anki Manual](https://docs.ankiweb.net/platform/linux/installing.html)
### Before
```shell
sudo apt install libxcb-xinerama0 libxcb-cursor0
```
### Steps
1. Descargar. Descarga la versión Qt6
   - [Anki - powerful, intelligent flashcards](https://apps.ankiweb.net/)
1. Descomprimir. Usa los comandos `tar xaf` en el archivo descargado dentro de la carpeta de descargas.
   ```shell
   tar xaf ./anki-2.1.XX-linux-qt6.tar.zst
   ```
1. Acceder a la carpeta. Ingresa a la carpeta que se acaba de descomprimir.
   ```shell
   cd anki-2.1.XX-linux-qt6
   ```
4. Ejecuta el instalador de Anki para Linux.
   ```shell
   sudo ./install.sh
   ```
## Extensiones
- **Shortcut:** `ctrl+shift+A`
- **Web de extensiones:** [Anki addons](https://ankiweb.net/shared/addons)
### Instalar extensiones
1. Ingresa a las extensiones de Anki dentro de la aplicación.
2. Haz click en el botón `obtener extensión`.
3. Copia el código de la extensión.
4. Reinicia Anki para activar la extensión.
### Review Heatmap
**Fuente:** [ankiweb.net/shared/info/1771074083](https://ankiweb.net/shared/info/1771074083)
```
1771074083
```
### AnkiConnect
**Fuente**: [ankiweb.net/shared/info/2055492159](https://ankiweb.net/shared/info/2055492159)
```
2055492159
```

#### To Read Pronunciation
1. Añade este enlace a la configuración de AnkiConnect.
   ```
   "http://127.0.0.1:8765",
   ```
2. Usa este formato dentro de la configuración de Read Pronunciation.
   - Palabra: `{{word}} /{{word.phonetic}}/`
   - Definición: `{{definitions}}`
   - Formas irregulares: `({{word.baseform}})`
   - Oración: `{{sentence}}`
   - Traducción: `{{sentence.translated}}`
   - Audio: `{{word.audio}}`
#### Obsidian-to-anki
1. Añade este enlace a la configuración de AnkiConnect:
   ```
   "app://obsidian.md",
   ```
## Añadir audio (solo para linux)
En linux debemos añadir una aplicación que permita a Anki reproducir audios, Anki nos recomienda 2 opciones:
- **mpv**: Es una aplicación completa con interfaz gráfica.
- **mplayer**: Por defecto es una aplicación de terminal, se le puede añadir una interfaz gráfica.

Personalmente me gusta la segunda, no añado toda la aplicación solo la parte que me interesa.
### Install mplayer
Copia el siguiente comando en la terminal:
   ```bash
   sudo apt install mplayer -y
   ```
