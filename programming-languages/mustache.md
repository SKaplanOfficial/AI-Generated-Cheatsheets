# Mustache Cheatsheet

Mustache is a logic-less template syntax used for web development. It provides a simple and flexible way to render data in a variety of formats, including HTML, XML, and JSON. This cheatsheet provides an overview of some of the key features of Mustache, along with code blocks for variables, loops, conditionals, and resources for further learning.

## Variables

```mustache
<!-- Rendering a variable -->
<p>{{ myVariable }}</p>

<!-- Rendering a nested variable -->
<p>{{ myObject.myProperty }}</p>

<!-- Rendering a variable with a default value -->
<p>{{ myVariable | 'Default Value' }}</p>
```

## Loops

```mustache
<!-- Rendering a list -->
<ul>
  {{# myArray }}
  <li>{{ name }}</li>
  {{/ myArray }}
</ul>

<!-- Rendering a list with a separator -->
<ul>
  {{# myArray }}
  <li>{{ name }}</li>{{/ myArray }}
</ul>

<!-- Rendering a list with an index -->
<ul>
  {{# myArray }}
  <li>{{ @index }}. {{ name }}</li>
  {{/ myArray }}
</ul>
```

## Conditionals

```mustache
<!-- Rendering a section if a variable is true -->
{{# isTrue }}
<p>This is true</p>
{{/ isTrue }}

<!-- Rendering a section if a variable is false -->
{{^ isFalse }}
<p>This is false</p>
{{/ isFalse }}
```

## Resources

- [Mustache documentation](https://mustache.github.io/)
- [Mustache tutorial](https://github.com/janl/mustache.js#usage)
- [Mustache.js library](https://github.com/janl/mustache.js/)