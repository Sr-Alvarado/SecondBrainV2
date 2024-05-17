---
{"dg-publish":true,"dg-path":"Como cambiar el tema global en KDE desde la terminal.md","permalink":"/como-cambiar-el-tema-global-en-kde-desde-la-terminal/","created":"2024-05-17T09:12","updated":"2024-05-17T09:12"}
---

Me encanta KDE, pero un problema es que me acostumbre al cambio automático entre tema claro y oscuro que ofrecía GNOME, en KDE, por lo menos yo, no encuentro como hacerlo. Por eso me puse a buscar como cambiar el tema a través de la consola para poder crear luego un script y automatizarlo con [[CRON\|CRON]], pero eso ya otro tema. Vamos a lo bueno:

Para cambiar el tema global en KDE solo debes usar:
```bash
lookandfeeltool -a <nombre_del_tema>
```
- `lookandfeeltool`. Es una herramienta de consola para cambiar rápidamente entre los temas globales y hacer que "look and feel".
- `-a`. Flag de `lookandfeeltool` que declara que se aplicará un nuevo tema.

Si no sabes el nombre del tema puedes usar:
```bash
lookandfeeltool -l
```
- `-l`. Flag de  `lookandfeeltool` que devuelve una lista de todos los temas instalados.