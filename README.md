## Countries.js

This is a simple JS library for populating dropdowns with countries and states / provinces.

## How To Use

To have a country select dropdown and a state / province select dropdown work together, where "country" is the id of your country select and "state" is the id of your state / province select, simply use:

```javascript
Countries.create("country", "state");
```

To manually populate a dropdown with a list of countries where "country" is the id of your target select element:

```javascript
Countries.fillCountries("country");
```

To manually populate a dropdown with a list of applicable states / provinces for a selected country where "state" is the id of
your target select element:

```javascript
var country = document.getElementById(countrySelectorId);
var value = country.options[country.selectedIndex].value;
Countries.fillStates("state", index);
```

## Example

To see this library in action, checkout the example.html file located at the root of the project's directory.
