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
<input type="text" ng-model="selected" typeahead="item for item in items | filter:$viewValue:$emptyOrMatch | limitTo:8" typeahead-focus class="form-control" >
```

## Trigger only if typeahead has value

There are number of cases when showing autocomplete for empty value does not make sense. 
However, when user enters a value in typeahead, leaves the field and then enters it again - 
typeahead should show the suggestions again.

If you want the `typeahead-focus` to trigger only when there is some entered value, add the `typeahead-focus-not-empty` attribute, i.e.:

```
<input type="text" ng-model="selected" typeahead="item for item in items" typeahead-focus typeahead-focus-not-empty class="form-control" >
```
