# Level 1
**Directive**: marker on a HTML tag that tells Angular to run or reference
some JavaScript code.
  - _ng-app_: se define en la etiqueta `html` indicando el módulo de angular que se ejecutará en esta página
  - _ng-controller_: define un controlador que se ejecutará dentro del bloque donde se defina. `ng-controller="nameController as alias"`
  - _ng-show_: mostrar un elemento cuando algo sea true
  - _ng-hide_: lo contrario
  - _ng-repeat_: repetir un bloque (div tipicamente). Util para repetir un bloque por cada uno de los elementos de un array `ng-repeat="element in controller.array"`

**Modules**: Piezas de cógigo Angular, donde se definen las dependencias. Sintaxis: ```angular.module("name", [deps]);```

**Controller**: Where define app's behaviour using functions and variables. Syntax ```module.controller('name', function(){ code to execute });```
