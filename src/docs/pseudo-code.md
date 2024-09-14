# Pseudo código para la página de inicio (index.astro)

1. **Importar el layout principal**.

   - Se usa para estructurar la página.

2. **Definir la página con un título**.

   - El layout envuelve el contenido de la página.

3. **Agregar contenido HTML**.

   - Mostrar un título, un párrafo estático y un párrafo que muestra la hora actual.

4. **Agregar JavaScript para actualizar la hora**.
   - Esperar a que el documento esté cargado.
   - Seleccionar el párrafo de la hora real.
   - Definir una función que actualiza la hora.
   - Actualizar la hora cada segundo.

# Pseudo código para componente CustomTitle

Inicio del componente CustomTitle:

1. Definir una interfaz llamada `Props`:

   - Tiene una propiedad llamada `title` de tipo string.
   - Esto indica que el componente espera recibir un valor llamado `title` que debe ser texto.

2. Recuperar la propiedad `title` desde `Astro.props`:

   - Usar la sintaxis de desestructuración para obtener `title` del objeto de propiedades.
   - El valor de `title` proviene de la página o componente que usa `CustomTitle`.

3. Generar la salida HTML:
   - Crear un elemento `h1` en el HTML.
   - Dentro del elemento `h1`, insertar el valor de `title`.

Fin del componente CustomTitle.

# Pseudo código para archivo about.astro

Inicio del archivo about.astro:

1. Importar los componentes:

   - Importar el componente `CustomTitle` desde la carpeta `components`.
   - Importar el layout `MainLayout` desde la carpeta `layouts`.

2. Usar el layout `MainLayout` para envolver el contenido de la página:

   - Pasar una propiedad `title` con el valor "About Page" al layout.

3. Dentro del layout:

   - Escribir un encabezado `h1` con el texto "About".
   - Usar el componente `CustomTitle`, pasándole una propiedad `title` con el valor "This is a custom title".

4. Definir los estilos locales:
   - Crear un bloque `<style>`.
   - Especificar que todos los elementos `h1` deben tener el color rojo.

Fin del archivo about.astro.
