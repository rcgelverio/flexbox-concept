Flexbox Concept
---------------
Compiled Resources on CSS Flexbox 

```
/* Set Flex Properties to container */
.container {
    display: -webkit-flex;
    display: -ms-flexbox;
    display: flex;
}
```

```
/* Set Flex Direction 
Properties: flex-direction: row | row-reverse | column | column-reverse;
*/
.container {
    -webkit-flex-direction: row reverse;
    -ms-flex-direction: row reverse;
    flex-direction: row-reverse;
}
````


```
/* Flex Wrap 
Properties: nowrap | wrap | wrap-reverse;
*/
.container {
    flex-wrap: nowrap; /* Default */
}
```

```
/* Justify Content 
Properties: justify-content: flex-start | flex-end | center | space-between | space-around;
*/
.container {
    justify-content: flex-start; /* Default */
}
```

```
/*
Align Contents
Properties: align-items: flex-start | flex-end | center | baseline | stretch;
.container {
    align-items: 
}
*/

```


###SCSS Prefixes
```
@mixin flexbox() {
  display: -webkit-box;
  display: -moz-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
}

@mixin flex($values) {
  -webkit-box-flex: $values;
  -moz-box-flex:  $values;
  -webkit-flex:  $values;
  -ms-flex:  $values;
  flex:  $values;
}

@mixin order($val) {
  -webkit-box-ordinal-group: $val;  
  -moz-box-ordinal-group: $val;     
  -ms-flex-order: $val;     
  -webkit-order: $val;  
  order: $val;
}

.wrapper {
  @include flexbox();
}

.item {
  @include flex(1 200px);
  @include order(2);
}
```


###Research Resources

[Flexbox Browser Support Chart](http://caniuse.com/flexbox)

[CSS Tricks: A Complete Guide to Flexbox](http://css-tricks.com/snippets/css/a-guide-to-flexbox/)

[Flexbox Cheatsheet](http://www.sketchingwithcss.com/samplechapter/cheatsheet.html)

[Solved by Flexbox](http://philipwalton.github.io/solved-by-flexbox/)

[Dive into Flexbox](http://bocoup.com/weblog/dive-into-flexbox/)

[Mozilla Developer Network: Using Flexible Boxes](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Flexible_boxes)

[Flexbox Grid: A Grid System based on Flexbox](http://flexboxgrid.com/)

[Gist: flexbox-mixins](https://gist.github.com/joseph-turner/5674311)
