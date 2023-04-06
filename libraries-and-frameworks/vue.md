# Vue Cheatsheet

Vue is a progressive framework for building user interfaces. It provides features such as reactive data binding, computed properties, directives, and component-based architecture to help developers build complex applications with ease. This cheatsheet provides an overview of some of the key features of Vue, along with code blocks for variables, functions, loops, conditionals, file manipulation, and resources for further learning.

## Variables

```vue
<template>
  <div>
    {{ myString }}
  </div>
</template>

<script>
export default {
  data() {
    return {
      myString: 'Hello, World!',
    };
  },
};
</script>
```

## Functions

```vue
<template>
  <div>
    <button @click="sayHello">Say Hello</button>
  </div>
</template>

<script>
export default {
  methods: {
    sayHello() {
      alert('Hello!');
    },
  },
};
</script>
```

## Loops

```vue
<template>
  <div>
    <ul>
      <li v-for="item in myArray" :key="item.id">{{ item.name }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      myArray: [
        { id: 1, name: 'Item 1' },
        { id: 2, name: 'Item 2' },
        { id: 3, name: 'Item 3' },
      ],
    };
  },
};
</script>
```

## Conditionals

```vue
<template>
  <div>
    <div v-if="isTrue">This is true</div>
    <div v-else>This is false</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isTrue: true,
    };
  },
};
</script>
```

## File manipulation

```vue
<template>
  <div>
    <my-component />
  </div>
</template>

<script>
import MyComponent from './MyComponent.vue';

export default {
  components: {
    MyComponent,
  },
};
</script>
```

## Resources

- [Vue documentation](https://v3.vuejs.org/guide/introduction.html)
- [Vue tutorial](https://v3.vuejs.org/guide/introduction.html)
- [Vue CLI](https://cli.vuejs.org/)
- [Vuex](https://vuex.vuejs.org/)
- [Vue Router](https://router.vuejs.org/)