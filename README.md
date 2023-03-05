# NgZoneRunOutsideMouseevent

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.2.1.

## INFO
Este proyecto presenta un ejemplo en el que se aplica el evento mousemove pero fuera de la zona de angular mediante NgZone (con esto no se activa la detección de cambios para dicho evento), con esto conseguiremos que no se esté refrescando constantemente la vista (renderizando) para mejorar así el rendimiento.
También en el ejemplo de los dos componentes (AppComponent y HelloComponent), existe el evento en el que se pulsa el botón (click), con esto vemos como se ejecuta dicho evento dentro de la zona de angular, por lo que como se tiene por en los componentes el cambio de deteccion por defecto, al darle click al botón de cualquiera de los dos componentes se puede apreciar en la consola que se renderiza todos y cada uno de los componentes (se aplica la detección por defecto, changeDetection: ChangeDetectionStrategy.Default), en la consola mostrará para cada vez que se haga un renderizado un correspondiente mensaje.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

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
