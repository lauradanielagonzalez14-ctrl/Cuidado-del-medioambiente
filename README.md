# Guardianes del Planeta

Sitio web interactivo de educacion ambiental. "Guardianes del Planeta" es una experiencia de una sola pagina (HTML, CSS y JavaScript) que combina teoria, contenido audiovisual, acciones y juegos para concientizar sobre el cuidado del medioambiente.

## Sitio desplegado

El proyecto se publica con GitHub Pages desde la rama principal:

[https://lauradanielagonzalez14-ctrl.github.io/Cuidado-del-medioambiente/](https://lauradanielagonzalez14-ctrl.github.io/Cuidado-del-medioambiente/)

## Materiales

Los tres materiales se encuentran en la raiz del repositorio. Los enlaces usan rutas relativas con espacios codificados como `%20` para que funcionen en GitHub Pages:

- Video introductorio: [video 1.mp4](video%201.mp4) — video introductorio que se reproduce con un sistema de precarga antes de la experiencia interactiva.
- Musica de fondo: [Audio 1.mpeg](Audio%201.mpeg) — musica de fondo que acompana la experiencia.
- Podcast: [podcast 1.mpeg](podcast%201.mpeg) — audio del podcast, accesible desde un boton etiquetado "podcast".

## Como funciona la experiencia

### Video introductorio con precarga

Al cargar la pagina aparece una capa a pantalla completa (`#intro-overlay`) con un precargador que muestra el mensaje "Cargando experiencia...". El boton "Comenzar" se habilita solo cuando los medios han terminado de precargarse.

Al pulsar "Comenzar" se reproduce el video introductorio [video 1.mp4](video%201.mp4) y comienza a sonar en bucle la musica de fondo [Audio 1.mpeg](Audio%201.mpeg). Cuando el video termina, o si el usuario pulsa "Saltar intro", la capa se oculta y se revela la experiencia interactiva. Un boton flotante permite silenciar o reactivar la musica de fondo.

Iniciar la reproduccion desde el boton "Comenzar" (una interaccion del usuario) es necesario porque los navegadores bloquean la reproduccion automatica de audio y video con sonido.

### Boton de podcast

En la seccion audiovisual hay un boton etiquetado exactamente "podcast" que activa y pausa la reproduccion del audio [podcast 1.mpeg](podcast%201.mpeg).

## Limitaciones conocidas

- El archivo [Audio 1.mpeg](Audio%201.mpeg) es actualmente un marcador de posicion vacio de 2 bytes, por lo que la musica de fondo sera silenciosa hasta que se reemplace por un archivo de audio real.
- El contenedor de audio `.mpeg` puede no reproducirse en todos los navegadores.
