# angular-tag-cloud
Create simple and clean tag clouds in angular with this library. This library is based on [Lucaong's jQCloud](https://github.com/lucaong/jQCloud) which is jQuery tag cloud library.

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

 
## Usage

In your html file, use the component like this:

```html
<ng-tag-cloud cloud-width="250" cloud-height="250" cloud-data="data"></ng-tag-cloud> <!-- default height and width is 300px -->
```
or with your custom defined `css`. Please check [code example](https://github.com/zeeshanhyder/angular-tag-cloud/tree/master/examples) to see how to implement custom `css`.

```html
<ng-tag-cloud class="custom-css-class" cloud-width="250" cloud-height="250" cloud-data="data"></ng-tag-cloud>
```

where your data is of `JSON` format as shown below. In your controller:

```javascript
$scope.data = [
          {text: "Lorem", weight: 15},
          {text: "Ipsum", weight: 9},
          {text: "Dolor", weight: 6},
          {text: "Sit", weight: 7},
          {text: "Amet", weight: 5}
          // ...as many words as you want
      ];
```

## Examples

Please check the examples directory to get the exact idea of what i am talking about. It's always better to check examples. 

Check code example [here](https://github.com/zeeshanhyder/angular-tag-cloud/tree/master/examples).

## Note

This is minimal version. Further versions will include custom `html` and `href` support. Thanks.