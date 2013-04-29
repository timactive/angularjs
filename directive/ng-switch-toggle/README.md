angularjs
=========

# ng-switch-toggle : angular module is compose 2  directive
  ng-switch-toggle-simple : simple switch
  ng-switch-toggle-group : switch multi choice

inspired by the excellent work of Ionut Colceriu( https://github.com/ghinda/css-toggle-switch), thank ;-)

__Contributors:__

timactive Team:
* [Romain Devera] (https://github.com/timactive)
 
Licensed under Unlicense 

Dependencies: jQuery & angular.js. 

***

## About
__ng-switch-toggle__

version 0.0.1 trunk

Questions, Comments, Complaints? feel free to email us at rdevera@timactive.com

***

## Roadmap

***
## How to use 
```html
<script type="text/javascript" src="angular.js"></script>
<script type="text/javascript" src="ng-switch-toggle.js"></script>
<!-- see https://github.com/ghinda/css-toggle-switch -->
<link  type="text/css" href="ng-switch-toggle.css" rel="stylesheet"/> 
<script>
    angular.module('myApp',['ngSwitchToggle', ... {other includes}]);
</script>
<body ng-app="myApp">
    <!--Simple switch toggle-->
<input type="checkbox" ng-switch-toggle-simple ng-model="simplechoice" text-on="Oui" text-off="Non" theme="candy"/>

<!--Complete choices -->
<ng-switch-toggle-group group-name="choicemonth2" theme="candy" ng-model="testradio2" choices="choices" color="yellow"></ng-switch-toggle-group>
</body>
```
```javascript
// Define your own controller somewhere..
function MyCtrl($scope) {
  $scope.choices = [ {
  									label : 'Hour',
										value : 'hour'
									},
									{
										label : 'Day',
										value : 'day'
									},{
										label : 'Week',
									value : 'week'
								}];
  $scope.simplechoice = true;
	// you can also specify data as: $scope.myOptions = { data: $scope.myData }. 
	// However, updates to the underlying data will not be reflected in the grid
};

```

## Examples
jsfiddle : 

## Testing




## Change Log
* __2013-04-29__ - Version 0.0.1B - first release 
