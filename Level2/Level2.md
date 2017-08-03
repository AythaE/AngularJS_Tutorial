# Level 2
**Filters**: Change or format expression output, it has the following syntax: `{{ data * | filter:options * }}`. There aree some built-in filters:
  - currency
  - date: `{{'1388123412323' | date:'MM/dd/yyyy @ h:mma'}}`
  - uppercase && lowercase: `{{'octagon gem' | uppercase}}`
  - limitTo: `{{'My Description' | limitTo:8}}` only prints the first 8 chars, this is also applicable to elements in an array.
  - orderBy: `ng-repeat="product in store.products | orderBy:'-price'"`, with - it order in descending order and WO it in ascending.

**Directives**:
  - _ng-src_: To load images from a module and evaluate the expresion before the page loads
  - _ng-click_: Change the value of an expression, defining a 2 way data binding (expresion reevaluates when a property changes)
  - _ng-init_: Allow to initiallize the value of an expression.
  - _ng-class_: Set a class for an html element with the following syntax `<element ng-class="{ classToApplicate:ExpressionToEval }"/>`
