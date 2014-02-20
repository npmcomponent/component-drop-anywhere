*This repository is a mirror of the [component](http://component.io) module [component/drop-anywhere](http://github.com/component/drop-anywhere). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/component-drop-anywhere`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# drop-anywhere

  Drag and drop files anywhere to upload.

## Installation

    $ component install component/drop-anywhere

## Example

```js
var dropAnywhere = require('drop-anywhere');

var drop = dropAnywhere(function(e){
  e.items.forEach(function(item){
    console.log(item);
  });
});
```

## API

### DropAnywhere#unbind()

  Unbind event handlers.

## Example CSS

  The classname `.show` is added when a user triggers a dragstart event. By
  default `#drop-anywhere` is stretched 100% horizontally and vertically, with
  a semi-transparent background.

```css
@-webkit-keyframes show {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

body {
  text-align: center;
}

#drop-anywhere {
  line-height: 500px;
  text-align: center;
  color: white;
  display: none;
}

#drop-anywhere::before {
  content: 'Drop to upload!';
}

#drop-anywhere.show {
  -webkit-animation: show 300ms;
}
  ```

## License

  MIT
