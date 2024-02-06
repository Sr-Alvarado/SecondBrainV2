---
{"dg-publish":true,"permalink":"/astro/","created":"2024-01-25T19:06","updated":"2024-02-04T19:57"}
---


## Uso
### Crear un nuevo proyecto
```bash
npm create astro@latest
```
- No es necesario crear una carpeta para el proyecto, astro la crea durante el proceso.
- Si quieres iniciar desde una plantilla remplaza `latest` por el nombre de la plantilla que quieres clonar.
### Actualizar la versión de astro
**Actualizar con `npx`**:
```bash
npx @astrojs/upgrade
```
**Actualizar con tu gestor de paquetes favorito**:
```bash
npm install astro@latest
pnpm upgrade astro --latest
yarn upgrade astro --latest
```
- Ejecuta este comando en la terminal dentro de tu proyecto y listo.
### Añadir integraciones
```bash
npx astro add INTEGRACION-1 INTEGRACION-2
```
- Puedes añadir varias integraciones a la ves.
- Añadiendo `--list` puedes ver todas las integraciones disponibles.
### Actualizar las extensiones
Proximamente...
### `.astro` - Crear un archivo Astro
Para definir una página como Astro guardas ese archivo con la extensión `.astro`.
### Importar y usar una plantilla o un componente
Dentro de el [[frontmatter\|frontmatter]] usamos la siguiente sintaxis:
```html
---
import Header from "../componets/Header.astro"
---
<Header>
```
- Indicamos que estamos importando con la palabra `import` y le asignamos un nombre al componente que queremos importar.
   - El nombre que asignemos será la forma en que llamemos a ese componente en nuestro archivo local.
   - El nombre debe iniciar con mayúscula para que astro sepa que se trata de un componente y no de alguna etiqueta [[Brain/Programation/HTML\|HTML]]. 
- Luego, con la palabra `from` indicamos de donde estamos importando y entre comillas dobles (`""`) escribimos la dirección del componente.
- Para usar el componente solo debemos llamarlo donde lo queramos usar como a cualquier etiqueta [[Brain/Programation/HTML\|HTML]] por el nombre que le asignamos.

### Iniciar un servidor de desarrollo
```bash
npm run dev
```
- Si quieres ver como evoluciona tu proyecto desde la web, ejecutando este comando podrás ver los cambios en vivo en este enlace: http://localhost:4321/
- Solo recuerda guardar tus cambios en [[vscode\|vscode]].

### Usar variables de componentes importados
**Header.astro**
```astro
---
const title = Astro.props;
---

<h1 id={`${title}`}>{title}</h1>
```
**Index.astro**
```astro
---
import Header from "../componets/Header.astro"
---

<Header title="Inicio">
```

- En la variable debemos definir las propiedades que queramos definir luego.
   - Si la variable va dentro de una etiqueta se coloca entre llaves (`{}`).
   - Si la variable va como una propiedad de la etiqueta se coloca con esta estructura: ``{`${name}`}``.
      - Las llaves exteriores declara que se va a escribir JS en Astro.
      - Las comillas reversas declaran que todo lo que está dentro es un string (`""`).
      - El símbolo `$` junto con las llaves declaran que lo que va dentro es una propiedad. 
- En el archivo local, luego de importar, en la etiqueta del componente importado definimos la propiedad.

