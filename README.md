## Countries.js

This is a simple JS library for populating dropdowns with countries and states / provinces.

## How To Use

To populate a dropdown with a list of countries where "country" is the id of your target select element:

```javascript
populateCountry("country");
```

To populate a dropdown with a list of applicable states / provinces for a selected country where "state" is the id of
your target select element: 

```javascript
var index = $("#country").val();
populateState("state", index);
```

You can place this code in an on change handler for the countries dropdown.

To populate the states / provinces without jQuery, use:

```javascript
var index = document.getElementById("country").selectedIndex;
populateState("state", index);
```
