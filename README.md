ngSwitch
=========
-allow to add or remove DOM elements
-work with ngSwitchcase & ngSwitchDefault
-similar to switch statement of js
-allow to display one or more DOM elements based on some pre-defined conditon
-place ngSwitchCase & ngSwitchDefault inside the ngSwitch directive
-Angular uses loose equality checks to compare the ngSwitchCase expression with the ngSwitch expression. This means that the empty string "" matches 0
-share the template between multiple ngSwitchCase using the ngTemplateOutlet
-can place one or more than one ngSwitchDefault anywhere inside the container element and not necessarily at the bottom.

Syntax
========
<container_element [ngSwitch]="switch_expression">
    <inner_element *ngSwitchCase="match_expresson_1">...</inner_element>
    <inner_element *ngSwitchCase="match_expresson_2">...</inner_element>
    <inner_element *ngSwitchCase="match_expresson_3">...</inner_element>
    <inner_element *ngSwitchDefault>...</element>
</container_element>


In app.module.ts
===================
import { FormsModule } from '@angular/forms';

@NgModule({
    imports: [
         FormsModule      
    ]


# NgswtichTest

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.0.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
