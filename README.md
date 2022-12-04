# b5toast
b5toast is javascript function to create and show bootstrap 5 toasts.

## Requirements

Add this html to the bottom(or anywhere) on the page. Only id is required. Classes can be changed according to your taste.

```html
<div class="position-fixed bottom-0 start-0 p-3" id="toast-container"></div>
<script defer src="/b5toast.js"></script>
```

## Demo
[Demo](https://auct.github.io/b5toast/b5toast_demo)


## Usage

#### Minimal

```javascript
b5toast.success('my message'); //show toast success
b5toast.error('my message'); //show toast danger
b5toast.show('warning', 'my message'); //show toast with warning/any bootstrap color
```

#### With optional title

```javascript
b5toast.success('my message', 'optional title'); //show toast success
b5toast.error('my message', 'optional title'); //show toast danger
b5toast.show('warning', 'my message', 'optional title'); //show toast with warning/any bootstrap color
```


#### With optional delay
Default delay is 7s, can be changed in b5toast.js file

```javascript
const optionalDelay = 1000;
b5toast.success('my message', 'optional title', optionalDelay);
b5toast.error('my message', 'optional title', optionalDelay);
b5toast.show('warning', 'my message', 'optional title', optionalDelay);
```