# Angular Notes

## Directives
**Directive**: marker on a HTML tag that tells Angular to run or reference some JavaScript code.

- _ng-app_: se define en la etiqueta `html` indicando el módulo de angular que se ejecutará en esta página
- _ng-controller_: define un controlador que se ejecutará dentro del bloque donde se defina. `ng-controller="nameController as alias"`
- _ng-show_: mostrar un elemento cuando algo sea true
- _ng-hide_: lo contrario
- _ng-repeat_: repetir un bloque (div tipicamente). Util para repetir un bloque por cada uno de los elementos de un array `ng-repeat="element in controller.array"`
- _ng-src_: To load images from a module and evaluate the expresion before the page loads
- _ng-click_: Change the value of an expression, defining a 2 way data binding (expresion reevaluates when a property changes)
- _ng-init_: Allow to initiallize the value of an expression.
- _ng-class_: Set a class for an html element with the following syntax `<element ng-class="{ classToApplicate:ExpressionToEval }"/>`

- _ng-model_: binds an html element to an angular element

- _ng-submit_: allow to call a function on a submited form

- _ng-include_: Insert another html into the current one, syntax `ng-include="'file.html'"`

- Custom: different types: Template expanding (Element and Attribute), events,...

## Modules
**Modules**: Piezas de cógigo Angular, donde se definen las dependencias. Sintaxis: `var app = angular.module("name", [deps]);`

## Controllers
**Controller**: Where define app's behaviour using functions and variables. Syntax `module.controller('name', [ dependencies like $http, $log..., function(dependencies){
} ]);`;

## Filters
**Filters**: Change or format expression output, it has the following syntax: `{{ data * | filter:options * }}`. There aree some built-in filters:

- currency
- date: `{{'1388123412323' | date:'MM/dd/yyyy @ h:mma'}}`
- uppercase && lowercase: `{{'octagon gem' | uppercase}}`
- limitTo: `{{'My Description' | limitTo:8}}` only prints the first 8 chars, this is also applicable to elements in an array.
- orderBy: `ng-repeat="product in store.products | orderBy:'-price'"`, with - it order in descending order and WO it in ascending.

## Expressions
**Expressions**: Pieces of Angular code (similar to plain JS code) that will be evaluated when the page loads, Syntax: `{{ exp }}`

## Additional Notes
It's a good practice to enclose all the angular code into this block
```(function() {
    AngularJS Code
})();```
