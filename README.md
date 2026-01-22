# Proyecto Application-Web-Design 
# Información del Estudiante
* **Nombre:** Joshua Jared Rosas Rico
* **Matrícula:** AL05055610
* **Carrera:** Ingeniería en Software
* **Semestre:** Sexto

# Información de la Materia
* **Materia:** Diseno Aplicaciones Web
* **Profesor:** Jesus Pegueros

# Markdown
 Markdown es un lenguaje de marcado ligero que se utiliza para crear texto con formato (como títulos, negritas o listas) de una manera muy sencilla. En GitHub se usa principalmente para documentar proyectos y crear archivos README que sean fáciles de leer tanto para humanos como para computadoras.
 
## Opciones de Etiquetado en Markdown

Markdown permite dar formato al texto de forma sencilla utilizando símbolos:

* **Negritas**: Se logra encerrando el texto entre doble asterisco como `**texto**`.
* *Cursivas*: Se logra usando un solo asterisco como `*texto*`.
* # Títulos: Se usan almohadillas (#) al inicio; una para título principal, dos para subtítulos.
* [Enlaces](https://google.com): Se pone el texto entre corchetes y el link entre paréntesis.
* `Código`: Se usan comillas invertidas para resaltar comandos o fragmentos de código.
* > Citas: Se usa el símbolo mayor que para crear bloques de texto resaltados.
* Listas: Se usan guiones (-) o asteriscos (*) para crear viñetas.

## Comandos de Git utilizados

En esta sección se listan los comandos fundamentales de Git para la gestión del repositorio:

### Consultar el estado del repositorio
Para verificar el estado de los archivos (saber si están en Stage, si tienen cambios o si el repositorio está limpio), se utiliza:

`git status`

### Agregar archivos al área de preparación (Stage)

Para preparar los archivos antes de realizar un commit, podemos hacerlo de dos formas:

* **De forma individual:** Permite elegir un archivo específico.
  `git add nombre_del_archivo`

* **De forma global:** Agrega todos los archivos con cambios en la carpeta actual de una sola vez.
  `git add .`

  ### Guardar cambios con un comentario (Commit)

Para registrar de forma permanente los archivos que están en el área de "Stage" y asignarles un mensaje descriptivo del cambio realizado:

`git commit -m "Tu mensaje descriptivo aquí"`

> **Nota:** El parámetro `-m` significa "message" (mensaje). Es una buena práctica escribir mensajes claros y breves en tiempo presente.    

### Gestión de Ramas (Branches)

Las ramas permiten trabajar en diferentes versiones de un proyecto de forma aislada:

* **Crear una rama:** Crea una nueva línea de tiempo para tus cambios.
  `git branch nombre-de-la-rama`

* **Listar ramas:** Muestra todas las ramas existentes y marca en cuál estás trabajando.
  `git branch`

* **Cambiar de rama:** Permite moverte entre las ramas creadas.
  `git checkout nombre-de-la-rama`

* **Eliminar una rama:** Borra una rama que ya no es necesaria (asegúrate de no estar dentro de ella al hacerlo).
  `git branch -d nombre-de-la-rama`


  ### Revertir cambios (Rollback)

Para regresar el repositorio a un estado anterior o a un commit específico, se utiliza el comando reset. Existen diferentes niveles, pero el más común para deshacer cambios es:

* **Regresar a un commit específico:**
  `git reset --hard id_del_commit`

> **Nota:** Para obtener el ID del commit (un código largo de números y letras), puedes usar el comando `git log`. Ten cuidado, ya que el parámetro `--hard` borrará todos los cambios que no hayan sido guardados después de ese commit.