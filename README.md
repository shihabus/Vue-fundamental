# Vue-fundamental

## Code

To instantiate Vue, define the root element in DOM where you want inject Vue. All things defined in `data` object can been access using flower braces inside the Vue component.

```
new Vue({
  el:'#root',
  data:{
    greeting:'Hello'
  }
})
```
```
<div id='root'>
  <h1>
    {{greeting}}
  </h1>
</div>
```
### Conditionals

#### v-if,v-else-if,v-else

Thye never end up in the dom until the condition is truthy

```
<div v-if="count === 1">
      Green
  </div>
  <div v-else-if="count === 2">
      Orange
  </div>
  <div v-else>
      Red
  </div>
```

#### v-show

They are added into the DOM, but their `display:none`

```
<div v-show="count==1">
     Dark Red
  </div>
```
