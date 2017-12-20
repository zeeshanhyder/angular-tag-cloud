# angular-tag-cloud
Create simple and clean tag clouds in angular with this library. This library is jQuery-less, for-angular port of [Lucaong's jQCloud](https://github.com/lucaong/jQCloud) library.

## Installation

### General
- Copy/move `ng-tag-cloud.js` from src dir in the package to your project dir
- In your Angular app, add a dependency to your module as below:
  
  `angular.module('yourApp',['ngTagCloud',...]');` 
  
### bower
In your project dir, type the following command:

```sh
$ bower install angular-tag-cloud
```
Then add a `<script>` in your project `html`:

```javascript
<script src='/bower_components/angular-tag-cloud/src/ng-tag-cloud.js'></script>
```
And finally in your Angular app, add the dependency as:

`angular.module('yourApp',['ngTagCloud',...]');`


### npm
In your project dir, run the following command:

```sh
$ npm install angular-tag-cloud
```
Then `require()` in your project source as:

```javascript
require('angular-tag-cloud')
```

### Styling

I have included a default `css` file for default styling. Include it in your file:

```html
<link rel="stylesheet" href="[bower_components | node_modules]/angular-tag-cloud/src/css/ng-tag-cloud.css">
```
You can easily override it with your custom `css` class.
 
## Usage

In your html file, use the component like this:

```html
<ng-tag-cloud cloud-width="250" cloud-height="250" cloud-data="data"></ng-tag-cloud> <!-- default height and width is 300px -->
```
or with your custom defined `css`. Please check [code example](https://github.com/zeeshanhyder/angular-tag-cloud/tree/master/examples) to see how to implement custom `css`.

```html
<ng-tag-cloud class="custom-css-class" cloud-width="250" cloud-height="250" cloud-data="data"></ng-tag-cloud>
```

You can also pass the font-sizes to make sure that the words not overlapping:

```html
<ng-tag-cloud weights="[ '100%' , '120%' , '160%' , '180%' ]"></ng-tag-cloud> 
``` 

you can use 'px' or 'rem' as well.

where your data is of `JSON` format as shown below. In your controller:

```javascript
$scope.data = [
          {text: "Lorem", weight: 15, link: "https://google.com"}, //if your tag has a link.
          {text: "Ipsum", weight: 9},
          {text: "Dolor", weight: 6},
          {text: "Sit", weight: 7},
          {text: "Amet", weight: 5}
          // ...as many words as you want
      ];
```

You can control whether there will be delay in word drawing like this:
```html
<ng-tag-cloud  cloud-width="250" cloud-height="250" delayed-mode="false"></ng-tag-cloud>
```
- True - 10 ms delay.
- False - No delay.
- Undefined - True only if there is more then 50 words.

You can pass function that will invoke after word cloud is rendered:
```html
<ng-tag-cloud  on-rendered="ctrl.myFunc()"></ng-tag-cloud>
```

## Examples

Please check the examples directory to get the exact idea of what i am talking about. It's always better to check examples. 

Check code example [here](https://github.com/zeeshanhyder/angular-tag-cloud/tree/master/examples).
