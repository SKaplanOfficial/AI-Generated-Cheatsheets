# AngularJS Cheatsheet

## Overview
- AngularJS is a JavaScript framework for building dynamic web applications.
- It uses a Model-View-Controller (MVC) architecture to organize code and provide separation of concerns.
- AngularJS is often used for single-page applications (SPAs) and is known for its two-way data binding and dependency injection.

## Directives
- Directives are markers on a DOM element that tell AngularJS to attach a specific behavior to that element.
- Directives can be used to create custom HTML tags, attributes, and classes.
- Some common directives include `ng-app`, `ng-model`, `ng-repeat`, and `ng-click`.

## Controllers
- Controllers are JavaScript functions that are responsible for controlling a part of the UI.
- Controllers can be used to set up the initial state of the scope, handle user input, and respond to events.
- Controllers can be defined using the `controller` method.

## Services
- Services are objects that provide functionality to an AngularJS application.
- Services can be used to share data between controllers, handle HTTP requests, and perform other common tasks.
- Services can be defined using the `service` method.

## Filters
- Filters can be used to format data for display in the UI.
- Some common filters include `currency`, `date`, `uppercase`, and `lowercase`.
- Filters can be chained together to create more complex transformations.

## Directives
- Directives are markers on a DOM element that tell AngularJS to attach a specific behavior to that element.
- Directives can be used to create custom HTML tags, attributes, and classes.
- Some common directives include `ng-app`, `ng-model`, `ng-repeat`, and `ng-click`.

## Example
```html
<!DOCTYPE html>
<html ng-app="myApp">
<head>
  <meta charset="UTF-8">
  <title>AngularJS Example</title>
</head>
<body ng-controller="myCtrl">
  <h1>Hello {{name}}!</h1>
  <p ng-repeat="item in items">{{item}}</p>
  <input type="text" ng-model="name">
  <button ng-click="addItem()">Add Item</button>

  <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.8.2/angular.min.js"></script>
  <script>
    var app = angular.module("myApp", []);
    app.controller("myCtrl", function($scope) {
      $scope.name = "World";
      $scope.items = ["Item 1", "Item 2", "Item 3"];
      $scope.addItem = function() {
        $scope.items.push("New Item");
      };
    });
  </script>
</body>
</html>
```

## Resources
- [AngularJS Website](https://angularjs.org/)
- [AngularJS Tutorial](https://docs.angularjs.org/tutorial)
- [AngularJS API Reference](https://docs.angularjs.org/api)