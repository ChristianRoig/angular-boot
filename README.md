# NgStarter
Este proyecto es un "proyecto inicial" Generado con Angular CLI, con algunos cambios menores detallados en doc/CHANGE-LOG.md

Un detalle de los pasos para su generacion puede encontrase en doc/STEPS.md

## Run in Development server

Ejecute `ng serve` para correr en un servidor de desarrollo. Navegue a `http://localhost:4200/`. La app se refresca automaticamente con cualquier cambio en los fuentes.

## Run with subpath in Development server

Si vamos a desplegar la app en un servidor web (apache), es probable que no querramos que el proyecto corra en la raiz del sitio “/” sino en un subdirectorio “/ngStarter”

para simular la misma ejecución que en apache desde el ambiente debemos usar:

`ng serve --serve-path /ngStarter/ --base-href /ngStarter/` 

y navegue a: `http://localhost:4200/ngStarter/`.

## Build
Nota: como no se instala en la raíz del apache (En nuestro caso lo vamos a instalar en ngStarter, el mismo nombre de la app) vamos a ejecutar 

`ng build --prod --base-href /ngStarter/` 

Nota: OJO, NO ejecutar con bash, sino con powershell o command

esto genera un carpeta ngStarter en dist que hay que colocar en htdocs de apache

## Deploy en Apache

copiar la carpeta ngStarter de dist dentro del htdocs de apache

y navegue a: `http://localhost/ngStarter/`.


# Origin 

## (de aqui en adelante se muestra el Readme Original de Angular CLI)

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.1.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
