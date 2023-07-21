![Logo de GammaTech School](./assets/Logo_Yellow.png)

# React ToDo App

#### [Aquí tenéis el proyecto desplegado para que os sirva como guía](https://chimerical-kelpie-0284f0.netlify.app/)

Ya hemos hecho otras aplicaciones de tareas, pero esta vez vamos a usar React para llevarlas al siguiente nivel. El objetivo es que nuestra ToDo App realice las siguientes tareas:
- guardar tareas.
- marcar tareas como cumplidas.
- eliminar tareas.
- guardar fecha de creación de la tarea y fecha de cumplimiento.
- ordenar tareas por fecha.
- añadir prioridad de tareas con colores predefinidos.
- añadir `tags` o etiquetas personalizadas con colores personalizados.
- menú de etiquetas para mostrar sólo las tareas de dicha categoría.

### Requisitos
- Git / GitHub
- React (estados)
- Tailwind
- Firebase

### Componentes mínimos
La aplicación debe contar con al menos los siguientes componentes (pueden tener más).
- `Form`: un formulario donde estén los `inputs` para introducir las tareas. Deberá conectarse, al menos, con `Firestore`` para actualizar la base de datos cuando se cree una tarea.
- `ToDoList`: el componente que renderizará la lista de tareas (componente `ToDo`).
- `ToDo`: cada una de las tareas. Recibirá la información por `props` desde el componente padre `ToDoList`.
- `TagsMenu`: este componente mostrará las `tags` introducidas por el usuario, y al hacer click en ellas, mostrará las tareas que coincidan con dicha `tag`. No olvides incluir una `tag` que permita ver todas.

### Iteraciones
Son muchas cosas, por lo que dividiremos el proyecto, como solemos hacer, en varias fases o iteraciones.
1. La primera iteración es la más básica: crear notas con botón de `delete` y de `done`. El primero eliminará la tarea; el segundo la marcará como completada (tachará el texto).
2. Añadir fechas de creación y de finalización que deben mostrarse en la `card` de la tarea.
3. Crear `select` para añadir prioridades (como mínimo `3`: alta, media y baja prioridad). Cada prioridad añadirá un color distintivo a la card de la tarea.
4. Crear botón para ordenar las notas por fecha (ascendente y descendente). Estos botones estarán en el componente `ToDoList`.
5. Añadir un nuevo `input` que permita generar un sistema de etiquetas. Este `input` aceptará texto y permitirá darle un nombre a la etiqueta ("trabajo", "clase", etc.). La etiqueta aparecerá dentro de la `card` de la tarea.
6. Añade un nuevo componente llamado `TagsMenu` que contenga todas las etiquetas o categorías de la aplicación. Cuando se haga click en una de ellas, se renderizarán exclusivamente las tareas que contengan dicha etiqueta.

### Consejos
1. Lo primero que deberías hacer es crear el repositorio en GitHub. Es importante que trabajes con `branches`, ya que conforme los proyectos se van complicando, es más fácil cometer un error fatal y que la aplicación deje de funcionar. Las ramas de git te ayudarán a evitar que eso ocurra.
2. Sigue las iteraciones en orden y **_leed bien el enunciado_**.
3. Las tareas deberán guardarse en un estado de React. Dado que habrá que guardar mucha información (texto, fecha, prioridad, etc.), cada tarea deberá ser un objeto necesariamente. Hazlo así desde el principio y no tendrás problemas más adelante cambiando código en distintos componentes.

![](https://media.giphy.com/media/RHOwWKH5OY7buuGHNi/giphy.gif)