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

   a. En VSC: haciendo clic en el nombre de la rama _main_ (abajo a la izquierda) e ingresando el nombre de la rama

   b. Por consola: {git checkout -b traducir}

2. Publicar la rama _traducir_.

   a. En VSC: junto al nombre de la rama nueva (abajo a la izquierda) se tiene un botón para publicar en la nube.
   
   b. Por consola: {git push -.set-upstream origin traducir} 
    
3. Resolver el requerimiento indicado arriba (siempre trabajando en la rama _traducir_).

4. Hacer los *commit* necesarios.

5. Hacer el *push*.

6. (desde la web del repo remoto) Generar el _pull request_ (PR) mediante el botón verde _New pull request_, y elegir un comentario descriptivo.

7. (desde la web) Aprobar el PR eligiendo _squash and merge_ en la lista desplegable.

8. (desde la web) Borrar la rama remota _traducir_. 

9. Cambiar localmente a la rama principal.

10. Hacer *pull*.

11. Borrar localmente la rama _traducir_.

