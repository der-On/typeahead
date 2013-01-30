# typeahead

typeahead widget

![typeahead](http://shtylman.github.com/typeahead/img.png)

## use

```javascript
var Typeahead = require('typeahead');

var input = document.createElement('input');

// source is an array of items
var ta = Typeahead(input, {
    source: ['foo', 'bar', 'baz']
});

input // =>
```

## options

### source
> array of values or function(query, result). Call result with array of return values.

```javascript
var Typeahead = require('typeahead');
var input = document.createElement('input');

// source is an array of items
var ta = Typeahead(input, {
    source: function(query, result) {
        result(['foo', 'bar', 'baz']);
    }
});

input // =>
```

### position
> location of the drop down menu. Valid values are ```above```, ```below```. default is ```below```

## style

Custom styling can be applied for the following rules.

### ul.typeahead
To style the list of suggestions.

### .typeahead.hidden
To style the hidden state of the menu

### .typeahead li
To style a li container.

### .typeahead a
To style the actual item text and selection area.

### .typeahead .active > a
To style the appearance of a selected item.

## License

The current code is fork of the bootstrap typeahead component and is licensed under [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
