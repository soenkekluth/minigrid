# CHANGELOG

### v2.0.0

The major change is that now minigrid receives a `props` object rather arguments.

```js
// v1.x
minigrid('.grid', '.grid-item');

// v2.0.0
minigrid({ container: '.grid', item: '.grid-item'});
```

On `window.onLoad` minigrid adds a new className, the container name plus the `--loaded` modifier.

```html
<div class="grid grid--loaded">
  ...
</div>
```

The same happens for each grid child item when it is ready for use.

```html
<div class="grid grid--loaded">
  <div class="grid-item grid-item--loaded">
</div>
```