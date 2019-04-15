# mocha-test
mocha-test

ref: https://mochajs.org/

# INSTALLATION
Install with npm globally:

```
$ npm install --global mocha
```


# GETTING STARTED

```
$ npm install mocha
$ mkdir test
$ $EDITOR test/test.js # or open with your favorite editor
```

In your editor:

~~~javascript
var assert = require('assert');
describe('Array', function() {
  describe('#indexOf()', function() {
    it('should return -1 when the value is not present', function() {
      assert.equal([1, 2, 3].indexOf(4), -1);
    });
  });
});
~~~

Back in the terminal:

```
$ ./node_modules/mocha/bin/mocha

  Array
    #indexOf()
      ✓ should return -1 when the value is not present


  1 passing (9ms)
```

Set up a test script in package.json:

~~~json
{
  "scripts": {
    "test": "mocha"
  }
}
~~~
Then run tests with:

```
$ npm test
```