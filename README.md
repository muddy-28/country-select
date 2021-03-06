# Country Select

A wrapper that replaces a `<select>` element with a JavaScript powered drop down with mini-flags.

![country select preview](http://i.imgur.com/lCdeAwm.png)

Check the demo in this repo.



## Usage

The `{countrycode}` variable is in the format specified in [ISO 3166-1 alpha-2](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).

``` html
<select name="country" class="flags">
	<option class="flag flag-{countrycode}">Country Name</option>
</select>
```

There is a custom-listener attached the selection of an item.

If your `<select>` has an `name` of `countries`:

``` javascript
$('input[name="countries"]').on('country-selected', function(){
    // ...
});
```

..or, if your `<select>` had an `id="countries"` property:

``` javascript
$('#countries').on('country-selected', function(){
    // ...
});
```


## Setup

`git clone https://github.com/WillemLabu/country-select && cd country-select`

`npm i && bower install`

`grunt init`

:{D

To build a minified & optimised version of the code, run `grunt` and check the `dist` directory.


## Attribution

Using the FamFamFam pack from [flag-sprites](http://www.flag-sprites.com/).

You can generate a new flag-sprite and CSS from that site and just replace the proper files.

## Licence

MIT
