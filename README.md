# svelte-stars-rating
## A Highly Customizable, easy-to-use elegant stars rating component
![MIT License](https://badgen.net/badge/license/MIT/blue "MIT License")
[![view on npm](http://img.shields.io/npm/v/svelte-stars-rating.svg?colorB=red)](https://www.npmjs.com/package/svelte-stars-rating)

###### Demo

![4.6 Star Rating](https://raw.githubusercontent.com/heithemmoumni/svelte-stars-rating/master/rating.png "3.6 Rating Stars")

[![Edit Vue Template](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/lively-https-ym9tj)

# Usage
Install via NPM ```npm i svelte-stars-rating```

Then require in your project:
```js
var StarRating = require('svelte-stars-rating');
```
or ES6 syntax:
```js
import StarRating from 'svelte-stars-rating'
```


You can then use the following selector anywhere in your project:
* To get up and running quick the package now supports rendering just the selector with default values
```html
<star-rating></star-rating>
```

## Basics

| Property | Type  | Description | Default
| --- | ---  | --- | --- |
| **rating** | Number  | A number between 0.0-5.0 that will determine the fullness of the 5-stars rating polygons | 1 |
| **isIndicatorActive** | Boolean | A property that deteremines weather a rating indicator would show to the right | true |

## Customized Styling

| Property | Type  | Description | Default |
| --- | ---  | --- | --- |
| **fullStarColor** | string | Set the full or partially-full star color | ```#ffd219``` |
| **emptyStarColor** | string | Set the empty or partially-empty star color | ```#737373``` |
| **styleStarWidth** | number | Set the star width | 20 |

## Implementation Example
Define your **config** options object in the component importing StarRating e.g
```js
const app = new App({
  target: document.body,
  props: {
    name: "svelte-stars-rating",
    rating: 4.7,
    isIndicatorActive: false,
    style: {
      styleStarWidth: 85,
      styleEmptyStarColor: "#737373",
      styleFullStarColor: "#ffd219"
    }
  }
})
```
or
```js
let style = {
   styleStarWidth: 85,
   styleEmptyStarColor: "#737373",
   styleFullStarColor: "#ffd219"
}
```
```html
<star-rating rating="4.7" style={style]></star-rating>
```
Feedback would be much appreciated, questions, suggestions, issues are more than welcome.

---

If you like to support my open-source contributions and feeling generous, feel free to:

<a href="https://www.buymeacoffee.com/Zukzhjx" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
