> **[danger] DEPRECATION WARNING**
>
> The Masked Input Plugin this component is based on is no longer in active development.  This field will be removed in v3.


# Masked input field
This is a masked input field for formatted string values. (e.g. phone number, zip code, card numbers...etc)

> Please note, this field depend on the following library:
- [jQuery](http://www.jquery.com)
- [maskedinput](http://digitalbush.com/projects/masked-input-plugin/)

## Special properties of field

Property      | Default  | Accepted values | Description
------------- | -------- | --------------- | -----------
`readonly`    | `false`  | `Boolean` 	   | If true, the input field is read only

## fieldOptions

Property      | Default  | Accepted values | Description
------------- | -------- | --------------- | -----------
`autocomplete` | _none_   | [see doc](https://html.spec.whatwg.org/multipage/forms.html#autofill)        | Indicates whether the value of the control can be automatically completed by the browser.
`mask`		  | _none_   | `String` 	   | Mask for input field (E.g. `(99) 999-9999`)
`maskOptions` | _none_   | `Object` 	   | Settings to masked component. [Read more info from options](http://digitalbush.com/projects/masked-input-plugin/)
`placeholder` | _none_   | `String` 	   | Placeholder text for input field

### maskOptions
@TODO
## Usage
#### Phone number masked field
```js
{
    type: "masked",
    label: "Mobile phone",
    model: "mobile",
    fieldOptions: {
        mask: "(99) 999-9999"
    }
}
```
#### Date masked field
```js
{
    type: "masked",
    label: "Date",
    model: "date",
    fieldOptions: {
      mask: "99/99/9999",
      placeholder: "mm/dd/yyyy"
    }
}
```
