# Branch-finder-and-template<!DOCTYPE html>


<html>


<head>

<script src= "http://ajax.googleapis.com/ajax/libs/angularjs/1.2.26/angular.min.js">
</script>

</head>


<body>



<div ng-app="" ng-controller="namesController">

<p>Filtering input:</p>


<p><input type="text" ng-model="test"></p>

<ul>
  <li ng-repeat="x in names | filter:test | orderBy:'country'">

    {{ (x.name | uppercase) + ', ' + x.country }}
  
</li>

</ul>


</div>


<script src="namesController.js"></script>

</body>
</html>
/*function namesController($scope) {
     $scope.names = [
         {name:'0263',country:'KIMBERLEY'},
         {name:'0046',country:'BANKCITY'},
         {name:'9874',country:'FNB SSC CENTRAL REGION 4'},*/
