# Sublime Snippets

A collection of [Sublime Text](http://www.sublimetext.com/) snippets

## Table of Contents

[Installation](#installation)
[Snippet List and Bindings](#snippet-list-and-bindings)
  - [Angular Snippets](#angular-snippets)
    - [Component Bindings](#angular-component-bindings)
    - [Components](#angular-components)
  - [Javascript Snippets](#javascript-snippets)
    - [Basic Bindings](#javascript-basic-bindings)
    - [Basics](#javascript-basics)
    - [Pattern Bindings](#javascript-pattern-bindings)
    - [Patterns](#javascript-patterns)

## Installation

Simply checkout the source code into Sublime Text's packages
directory. The location is system specific specific

#### For OSX

    $ cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/
    $ git clone git://github.com/matthewrobertson/ERB-Sublime-Snippets.git ERB_Snippets

#### For Windows

    $ cd %APPDATA%/Sublime Text 2/Packages/
    $ git clone git://github.com/matthewrobertson/ERB-Sublime-Snippets.git ERB_Snippets

#### For Linux

    $ cd ~/.Sublime Text 2/Packages/
    $ git clone git://github.com/matthewrobertson/ERB-Sublime-Snippets.git ERB_Snippets

## Snippet List and Bindings

#### Angular Snippets

##### *Angular Component Bindings*

| Snippet               | Binding               |
| --------------------- | --------------------- |
| Config                | ng-configuration      |
| Constant              | ng-constant           |
| Controller            | ng-controller         |
| Directive             | ng-directive          |
| Factory               | ng-factory            |
| Filter                | ng-filter             |
| Run                   | ng-run                |
| Service               | ng-service            |
| Value                 | ng-value              |

##### *Angular Components*

###### Angular Configuration

    (function() {

      'use strict';

      angular
        .module('app')
        .config(Configuration);

      Configuration.$inject = [

      ];

      function Configuration(

      ) {

        // function body

      }

    })();

###### Angular Constant

    (function() {

      'use strict';

      angular
        .module('app')
        .value('constant', 'value');

    })();

###### Angular Controller

    (function() {

      'use strict';

      angular
        .module('app')
        .controller('controllerController', Controller);

      Controller.$inject = [

      ];

      function Controller(

      ) {

        var vm = this;

        vm.property = 'value';

        return vm;

      }

    })();

###### Angular Directive

    (function() {

      'use strict';

      angular
        .module('app')
        .directive('appComponent', Directive);

      Directive.$inject = [

      ];

      function Directive(

      ) {

        var directive = {
          templateUrl: '/templates/component.tpl.html',
          restrict: 'E'
        };

        return directive;

      }

    })();

###### Angular Factory

    (function() {

      'use strict';

      angular
        .module('app')
        .factory('factoryFactory', Factory);

      Factory.$inject = [

      ];

      function Factory(

      ) {

        var factory;

        factory = {
          property: property
        };

        return factory;

        function property() {

          // function body

        }

      }

    })();

###### Angular Filter

    (function() {

      'use strict';

      angular
        .module('app')
        .filter('filterFilter', Filter);

      Filter.$inject = [];

      function Filter() {

        return function(args) {
          return true;
        };

      }

    })();

###### Angular Run

    (function() {

      'use strict';

      angular
        .module('app')
        .run(Run);

      Run.$inject = [

      ];

      function Run(

      ) {

        // function body

      }

    })();

###### Angular Service

    (function() {

      'use strict';

      angular
        .module('app')
        .service('serviceService', Service);

      Service.$inject = [

      ];

      function Service(

      ) {

        var service;

        service = {
          property: property
        };

        return service;

        function property() {

          // function body

        }

      }

    })();

###### Angular Value

    (function() {

      'use strict';

      angular
        .module('app')
        .value('value', 'value');

    })();

#### Javascript Snippets

##### *Javascript Basic Bindings*

| Snippet               | Binding               |
| --------------------- | --------------------- |
| Anonymous Function    | js-anonymous-function |
| For Each              | js-for-each           |
| For In                | js-for-in             |
| For Loop              | js-for-loop           |
| Function              | js-function           |
| Immediately Invoked   | js-iife               |
| Object Keys           | js-object-keys        |
| Prototype             | js-prototype-function |

##### *Javascript Basic Binding*

###### Javascript Anonymous Function

    function (args) {

        // body...

    }

###### Javascript For Each

    array.forEach(function(element) {

        // body...

    });

###### Javascript For In

    for (var property in object) {

      if (object.hasOwnProperty(property)) {
        // body...
      }

    }

###### Javascript For Loop

    for (i = 0, len = array.length; i < len; i++) {

      // body...

    }

###### Javascript Function

    function methodName (args) {

        // body...

    }

###### Javascript Immediately Invoked Function Expression

    (function(){

      'use strict';

      // body

    })();

###### Javascript Object Keys

    Object.keys(object).forEach(function (key) {

        // body...

    });

###### Javascript Prototype Function

    ClassName.prototype.methodName = function(args) {

        // body...

    };

##### *Javascript Pattern Bindings*

| Snippet               | Binding               |
| --------------------- | --------------------- |
| Constructor           | js-contructor         |
| Module                | js-module             |
| Namespace             | js-namespace          |
| Singleton             | js-singleton          |

##### *Javascript Patterns*

###### Javascript Constructor Pattern

    var ConstructorName = (function() {

      'use strict';

      function ConstructorName(args) {

        // enforces new
        if (!(this instanceof ConstructorName)) {
            return new ConstructorName();
        }

        // constructor body

      }

      ConstructorName.prototype.methodName = function(args) {

        // method body

      };

      return ConstructorName;

    }());

###### Javascript Module Pattern

    var moduleName = (function() {

      'use strict';

      var moduleName = {

        init: {
          // initialize
        }

      };

      return moduleName;

    }());

###### Javascript Singleton Pattern

    var singletonName = (function() {

      'use strict';

      var instance;

      singletonName = function() {

        if (instance) {
          return instance;
        }

        instance = this;

        // singleton body

      };

      return singletonName;

    }());

###### Javascript Namespace Pattern

    (function(namespace) {

      'use strict';

      namespace.method = function() {

        // function body

      };

    })(window.namespace = window.namespace || {});


## Author
email: [jech@boolex.com](jech@boolex.com) <br />
twitter.com: [@jervenclark](http://twitter.com/jervenclark) <br />
github: [github.com/jervenclark](https://github.com/jervenclark) <br />

## License

Released under the [MIT License (MIT)](http://opensource.org/licenses/MIT)

Copyright (c) 2014 Geekhero

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
