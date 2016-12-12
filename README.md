# Handlebars.js Conditional Helper function
This is a simple set of helper functions for the Handlebars.JS template library.

## Usage
### Equal - eq
```html
{{#if (eq direction "left")}}
<!-- If the value of the direction property equals "l" -->
<div>{direction}</div>
{{else}}
<div>right</div>
{{/if}}
```
### Not Equal = ne
```html
{{#if (ne direction "left")}}
<!-- If the value of the direction property does not equals "l" -->
<div>right</div>
{{else}}
<div>{direction}</div>
{{/if}}
```

### Less Than - lt
```html
{{#if (lt number 20)}}
<!-- If the value of the number property is less than 20 -->
<div>{number} is less than 20</div>
{{else}}
<div>{number} is greater than 20</div>
{{/if}}
```

### Greater Than - gt
```html
{{#if (gt number 20)}}
<!-- If the value of the number property is greater than 20 -->
<div>{number} is greater than 20</div>
{{else}}
<div>{number} is less than 20</div>
{{/if}}
```

### Less Than or Equal - lte
```html
{{#if (lte number 20)}}
<!-- If the value of the number property is less than or equal to 20 -->
<div>{number} is less or equal to than 20</div>
{{else}}
<div>{number} is greater than or equal to 20</div>
{{/if}}
```

### Greater Than or Equal - gte
```html
{{#if (gte number 20)}}
<!-- If the value of the number property is greater than or equal to 20 -->
<div>{number} is greater than or equal to 20</div>
{{else}}
<div>{number} is less or equal to than 20</div>
{{/if}}
```

### And - and
```html
{{#if (and number letter)}}
<!-- If the value of the number AND letter are both truthy -->
<div>There are {number} of the {letter}</div>
{{else}}
<div>There are no letters that mater {letter}</div>
{{/if}}
```

### Or - or
```html
{{#if (or colorOne colorTwo)}}
<!-- If the value of the number OR letter are truthy -->
<div>One of the colors exists</div>
{{else}}
<div>Neither of the colors exists</div>
{{/if}}
```
