# angular-tag-cloud
Create colorful cloud tags in angular with this library. No dependencies. This library is based on [Lucaong's jQCloud](https://github.com/lucaong/jQCloud) which is jQuery based tag cloud library.

## Installation

- Copy/move `ng-tag-cloud.js` from src dir in the package to your project dir
- In your Angular app, add a dependency to your module as below:
  
  `angular.module('yourApp',[ngTagCloud]');`
  
> **`NPM`** Support coming soon!
  
## Usage

In your html file, use the component like this:

```html
<ng-tag-cloud cloud-width="250" cloud-height="250" cloud-data="data"></ng-tag-cloud> <!-- default height and width is 300px -->
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