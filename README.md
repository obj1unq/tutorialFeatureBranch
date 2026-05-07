# Tutorial: creación de ramas por requerimiento (o _Feature Branchs_)

## Feature Branch

El protocolo GIT tiene diferentes formas de trabajo grupal (workflows). Uno de estos es el _features branch workflow_, que propone usar una branch (rama) por cada tarea, y así poder dividir el trabajo en tareas pequeñas. Además tiene en cuenta lo siguiente:

* Una _feature branch_ se crea a partir de la rama
principal (main o master)

* Todos los commits/pushs se realizan sobre la
_feature branch_.

* Nunca se realizan commits directamente sobre la
rama principal

* Al finalizar la tarea, se integran los cambios a la
rama principal a través de un *_Pull Request_*

* Luego de integrado, la _feature branch_ se descarta


## Ejercicio

*Requerimiento*: traducir al castellano el código disponible en los archivos pepita.wlk y testPepita.wtest

*Metodología* 

1. Crear una _feature branch_ con el nombre _"traducir"_ (quedando esta rama como la rama actual o _current_).
2. Publicar la rama _traducir_.
3. Resolver el requerimiento indicado arriba (siempre trabajando en la rama _traducir_).
4. Hacer los *commit* necesarios.
5. Hacer el *push*.
6. Generar el _pull request_ (PR) desde la web del repositorio remoto correspondiente en Github.
7. (desde la web) Aprobar el PR haciendo _squash and merge_.
8. (desde la web) Borrar la rama remota _traducir_. 
9. Cambiar localmente a la rama principal.
10. Hacer *pull*.
11. Borrar localmente la rama _traducir_.

