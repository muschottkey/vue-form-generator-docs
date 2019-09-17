# spectrum field
This is a "The No Hassle" color picker  component.

> Please note, this field depend on the following library:
- [jQuery](http://www.jquery.com)
- [spectrum](https://github.com/bgrins/spectrum)

## Special properties of field

Property        | Default  | Accepted values | Description
--------------- | -------- | --------------- | -----------
`fieldOptions`  | `{}`     | `Object` 		 | Settings to picker. [Read more info from options](http://bgrins.github.io/spectrum/)
`placeholder`   | _none_   | `String` 	     | Placeholder text for input field
`readonly`      | `false`  | `Boolean` 	    | If true, the input field is read only

### `fieldOptions`

Property        | Default  | 	Accepted values | Description
--------------- | -------- | 	--------------- | -----------
`autocomplete` 	| _none_   | [see doc](https://html.spec.whatwg.org/multipage/forms.html#autofill)         | Indicates whether the value of the control can be automatically completed by the browser.
`color` 				| `value`  | `tinycolor` 			| Initial color. [See doc](http://bgrins.github.io/spectrum/#options-color)
`flat`					| `false`  | `Boolean`				| This means that it will always show up at full size, and be positioned as an inline-block element
showInput				| `true`	 | `Boolean`				| You can add an input to allow free form typing. [See doc](http://bgrins.github.io/spectrum/#options-showInput)
showInitial			| `false`  | `Boolean`				| Spectrum can show the color that was initially set when opening. [See doc](http://bgrins.github.io/spectrum/#options-showInitial)

For more options, see http://bgrins.github.io/spectrum/#options

## Usage

```js
{
    type: "spectrum",
    label: "Color",
    model: "favoriteColor",
    fieldOptions: {
       preferredFormat: "rgb"
    }
}
```
