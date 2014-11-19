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
.site-data {
    background: white;

    @include phone {
        background: red;
        
        @include landscape {
            color: green;
        }
    }
    
    @include tablet {
        background: yellow;
        
        @include landscape {
            color: violet;
        }
    }
    
    @include desktop {
        background: blue;
    }
}
```
