# Starter ANGULAR - Paso a Paso (del comienzo)

## Etapa 1 (creando el proyecto)

### 1.- Instalar Node, npm y angular cli
(ref: https://angular.io/guide/setup-local ) 

`ng version`

    Angular CLI: 12.1.3

    Node: 16.5.0 (Unsupported)

    Package Manager: npm 7.19.1

    OS: darwin arm64

### 2.- Crear un proyecto con Angular CLI y ejecutarlo. 

`ng new starter-front-angular`

    ? Would you like to add Angular routing? Yes

    ? Which stylesheet format would you like to use? CSS

    CREATE starter-front-angular...

    Packages installed successfully.

    Successfully initialized git.

`cd starter-front-angular`

`ng serve -o`

    Compiled successfully.

### 3.- Instalar GIT, verificar version e initialize

(la instalacion de node a veces ya instala e inicializa git)

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

### 6.- Subir a la nuebe (opcional)
Pero antes de empezar podemos crear un repositorio en la nube (por ejemplo en GitHub) y subir nuestro proyecto al repositorio remoto (este paso también lo podemos hacer más adelante)

`git remote add origin https://github.com/Siete-Ideas/starter-front-angular`

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

### 3.1.- Ejecuto en “/starter”

para simular la misma ejecución que en apache desde el ambiente de desarrollo debemos usar:

`ng serve --serve-path /starter/ --base-href /starter/`

y accedemos con http://localhost:4200/starter/ 

### 3.2.- Build
Nota: como no se instala en la raíz del apache (En nuestro caso lo vamos a instalar en ngStarter, el mismo nombre de la app) vamos a ejecutar: 

`ng build --prod --base-href /starter/` 

Nota: OJO, NO ejecutar con bash, sino con powershell o command

Nota: esto genera un carpeta starter en dist que hay que colocar en htdocs de apache

### 3.3.- hacer deploy en Apache
Copiar la carpeta starter de dist dentro del htdocs de apache

Nota: este texto se agrega al readme del proyecto

### Bonus
Se puede agregar el link al repositorio del proyecto.


