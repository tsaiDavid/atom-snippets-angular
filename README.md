# atom-snippets-angular

@cyung developed these snippets for use in Sublime Text. Being an Atom user, I simply converted them into the `.cson` (CoffeeScript-Object-Notation) format that Atom uses.

##Installation

Clone this repo and simply place the snippets you want to use into the `snippets.cson` file in Atom. Please keep in mind that you can only have one source (ex: `'source.js'`) listed at any given time, so stack them on accordingly!

***Here's what Atom has to say about using their snippets:***

>There is a text file in your ~/.atom directory called `snippets.cson` that contains all your custom snippets that >are loaded when you launch Atom. However, you can also easily open up that file by selecting the Atom > Open Your >Snippets menu.

## Examples
```
a-app

angular.module('app', ['']);
```

```
a-ctrl

(function() {
  'use strict';

  angular.module('app')
  .controller('<Name>Ctrl', <name>Ctrl);

  function <name>Ctrl() {
    var self = this;

    
  }

})();
```

```
a-fact

(function() {
  'use strict';

  angular.module('app')
  .factory('<name>Factory', <name>Factory);

  function <name>Factory() {
    var services = {
      <function name>: <function name>
    };

    return services;

    function <function name>() {
      
    }
  }

})();
```

```
a-dir

(function() {
  'use strict';

  angular.module('app')
  .directive('<name>', <name>);

  function <name>() {
    var directive = {
      template: '',
      link: link
    };

    return directive;

    function link(scope, elem, attrs) {
      
    }
  }

})();
```
