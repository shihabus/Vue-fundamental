# Vue-fundamental

## Code

```
new Vue({
  el:'#root',
  data:{
    greeting:'Hello'
  }
})
```

### v-if,v-else-if,v-else

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

### v-show

They are added into the DOM, but their `display:none`

```
<div v-show="count==1">
     Dark Red
  </div>
```
