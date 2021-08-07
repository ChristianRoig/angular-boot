# NgStarter - Paso a Paso
Este proyecto es un "proyecto inicial" Generado con Angular CLI, con algunos cambios menores detallados en doc/CHANGELOG.md

Un detalle de los pasos para su generacion puede encontrase en doc/STEPS.md

## Run in Development server

## Pasos (Etapa 1, creando el proyecto)

### 1.- Instalar Node, npm y angular cli( https://angular.io/guide/setup-local ) 

`ng versión`
Angular CLI: 12.1.3
Node: 16.5.0 (Unsupported)
Package Manager: npm 7.19.1
OS: darwin arm64

### 2.- Crear un proyecto con Angular CLI y ejecutarlo. 

`ng new ngStarter`
? Would you like to add Angular routing? Yes
? Which stylesheet format would you like to use? CSS
CREATE ngStarter...
✔ Packages installed successfully.
Successfully initialized git.

`cd ngStarter`

`ng serve -o`
	✔ Compiled successfully.

### 3.- Instalar GIT, verificar version e initialize (en gral esta hecho)
`git version`
	git version 2.30.1 (Apple Git-130)

### 4.- Resguardar código de origen en una rama y crear rama starter
`git checkout -b bak-origin`
`git checkout -b starter`
`git branch`
  	bak-origin
  	master
    * starter

### 5.- Instalar VSCode, abrir el proyecto de Angular CLI y ejecutarlo. 

Listo! ya estamos en condiciones de empezar a trabajar en nuestra rama starter.

### 6.- Pero antes de empezar podemos crear un repositorio en la nube (por ejemplo en GitHub) y subir nuestro proyecto al repositorio remoto (este paso también lo podemos hacer más adelante)
`git remote add origin https://github.com/ChristianRoig/ngStarter.git`
`git branch -M master`
`git push master origin`
`git push --all origin`


## Pasos (Etapa 2, modificando el proyecto)
2.1.- Cambio el README.md
2.2.- Versiono el html y apunto el componente a la v1.
2.3.- Recorte mínimo (comento el footer)
2.4.- Termino de recortar (comento otras secciones)
2.5.- Traduzco y adapto el html.

Listo! ya terminamos los cambios

`git push`

## Pasos (Etapa 3, corriendo el proyecto)

Vamos a desplegar la app en un servidor web (apache) pero es probable que no querramos que el proyecto corra en la raiz del sitio “/” sino en “/ngStarter”

### 3.1.- Ejecuto en “/ngStarter”

para simular la misma ejecución que en apache desde el ambiente de desarrollo debemos usar:
`ng serve --serve-path /ngStarter/ --base-href /ngStarter/`

y accedemos con http://localhost:4200/ngStarter/ 

### 3.2.- Build
Nota: como no se instala en la raíz del apache (En nuestro caso lo vamos a instalar en ngStarter, el mismo nombre de la app) vamos a ejecutar 
`ng build --prod --base-href /ngStarter/` 

Nota: OJO, NO ejecutar con bash, sino con powershell o command

esto genera un carpeta ngStarter en dist que hay que colocar en htdocs de apache

### 3.3.- hacer deploy en Apache
copiar la carpeta ngStarter de dist dentro del htdocs de apache

Nota: este texto se agrega al readme del proyecto

### Bonus
Se puede agregar el link al repositorio del proyecto.


