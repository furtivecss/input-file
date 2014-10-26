# Furtive Input File

A CSS module for styling file inputs: `input[type="file"]`. Used in [furtive.css](http://furtive.co).

## Installation

It's recommended to use [rework-npm](https://github.com/reworkcss/rework-npm):

```
npm install --save furtive-file-input
```

```javascript
var rework = require('rework'),
    reworkNPM = require('rework-npm');

var output = rework('@import "furtive-file-input";', { source: 'my-file.css' })
    .use(reworkNPM());
```

## Usage

Replacing the default 'Choose File' button with a camera icon:

```html
<div class="input--file">
  <span>
    <i class="ic ic-camera"></i>
  </span>
  <input name="Select File" type="file" />
</div>
```

_Note:_ This will also hide the filename when a file is selected, as that is part of the file
input. A dash of Javascript will be required to allow the filename to be visible.

Detailed documentation and examples can be found at [furtive.co](http://furtive.co).

## License

MIT

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

Crafted with <3 by [John Otander](http://johnotander.com) ([@4lpine](https://twitter.com/4lpine)).
