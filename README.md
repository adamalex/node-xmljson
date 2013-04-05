# rerender

Translates between JSON and XML formats

## Getting Started
Install the module with: `npm install rerender`

### Convert XML to JSON

```javascript
// Load the module
var to_json = require('rerender').to_json;

// An XML string
var xml = '' +
	'<data>' +
		'<prop1>val1</prop1>' +
		'<prop2>val2</prop2>' +
		'<prop3>val3</prop3>' +
	'</data>';

to_json(xml, function (error, data) {
	// Module returns a JS object
	console.log(data);
	// -> { prop1: 'val1', prop2: 'val2', prop3: 'val3' }

	// Format as a JSON string
	console.log(JSON.stringify(data));
	// -> {"prop1":"val1","prop2":"val2","prop3":"val3"}
});
```
## Release History

_This module is semantically versioned: <http://semver.org>_

### Version 0.1.0 `2013-01-26`

* Initial release

## Contributing
Before writing code, we suggest you [search for issues](https://github.com/ExactTarget/node-rerender/issues?state=open)
or [create a new one](https://github.com/ExactTarget/node-rerender/issues/new) to confirm where your contribution fits into
our roadmap.

In lieu of a formal style guide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality.
Lint and test your code using [grunt](https://github.com/cowboy/grunt).

##Authors

**Adam Alexander**

+ http://twitter.com/adamalex
+ http://github.com/adamalex

## Copyright and license

Copyright (c) 2013 ExactTarget

Licensed under the MIT License (the "License");
you may not use this work except in compliance with the License.
You may obtain a copy of the License in the COPYING file.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
