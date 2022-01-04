Angular JS
     AngularJS is a JavaScript framework. It can be added to an HTML page with a <script> tag,Directives and Expression.
Script Tag
  <script src="https//docs.anugularjs"></script>
Ng directives:
  ng directive defines an AngularJS application.
  ng-model directive binds the value of HTML controls (input, select, textarea) 
  ng-bind directive binds application data to the HTML view.
Eg:
  <!DOCTYPE html>
   <html>
  <script src="https//docs.angularjs"></script>
  <body>
  <div ng-app="">
  <p>Name: <input type="text" ng-model="name"></p>
  <p ng-bind="name"></p>
   </div>
   </body>
    </html>
 Ng-init:
    ng-init directive initializes AngularJS application variables.
  Eg:
    <div ng-app="" ng-init="firstName='Angular JS'">
    <p>The name is <span ng-bind="firstName"></span></p>
    </div>
  Expression:
     AngularJS expressions are written inside double braces: {{ expression }}
  Eg:
     <!DOCTYPE html>
     <html>
     <script src="https://docs angular js"></script>
     <body>
     <div ng-app="">
     <p>Expression {{ 5 + 5 }}</p>
     </div>
     </body>
     </html>
  Angular Modules:
      The module is a container for the different parts of an application.The module is a container for the application controllers
  Eg:
     <div ng-app="myApp">...</div>
     <script>
     var app = angular.module("myApp", []);
      </script>
  Modules and Controllers:
     It is common in AngularJS applications to put the module and the controllers in JavaScript files
  Eg:
     <!DOCTYPE html>
     <html>
     <script src="https://docs angular js"></script>
     <body>
     <div ng-app="myApp" ng-controller="myCtrl">
     {{ firstName + " " + lastName }}
     </div>
     <script src="myApp.js"></script>
     <script src="myCtrl.js"></script>
      </body>
      </html>
  myApp.js:
      var app = angular.module("myApp", []);
  myCtrl.js:
      app.controller("myCtrl", function($scope) {
      $scope.firstName = "Pandi";
      $scope.lastName= "Selvi";
      });
  Global Namespace:
       Global functions should be avoided in JavaScript. They can easily be overwritten or destroyed by other scripts.
  AngularJS Directives:
        AngularJS directives are extended HTML attributes with the prefix ng-
  Types:
      ng-app
      ng-module
      ng-init
  Data Binding:
     Data binding in AngularJS binds AngularJS expressions with AngularJS data.
     {{ firstName }} is bound with ng-model="firstName".
  
  
