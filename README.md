# Typeahead Focus - Add a focus functionality to Angular UI Bootstrap Typeahead

This project is intended to add a "focus" functionality to the [angular-ui-bootstrap](https://github.com/angular-ui/bootstrap) 
typahead directive. It activates the typeahead's menu on click in addition to the default keyboard initiated functionality.

## Installation

```bower install typeahead-focus --save```

##Usage
```
// Add 'typeahead-focus' dependency to your app
var myApp = angular.module('myApp', ['typeahead-focus']);
```
```
<!-- Use the 'input' element as follows -->
<input type="text" ng-model="selected" typeahead="item for item in items | filter:$viewValue:emptyOrMatch | limitTo:8" typeahead-focus class="form-control" >
```