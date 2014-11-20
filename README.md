# semantic-query - *media queries by purpose, not by numbers*

Semantic Query is a Sass library for the impatient -- those who just simply want a sane context for their CSS properties without any hassle. The initial version of Semantic Query provides its users with three separate screen size related mixin utilities:

* phone
* tablet
* desktop

and two auxiliary mixins for orientation:

* portrait
* landscape

## Example usage

```
@import 'semantic-query';

body {
  background-color: green;

  @include phone {
    background-color: red;
    @include landscape {
      background-color: orange;
    }
  }

  @include tablet {
    background-color: yellow;
    @include landscape {
      background-color: green;
    }
  }

  @include desktop {
    background-color: blue;
    @include portrait {
      background-color: violet;
    }
  }
}
```
