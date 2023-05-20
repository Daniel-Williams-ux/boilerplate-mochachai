# Quality Assurance with Chai

This is the boilerplate for the Quality Assurance with Chai lessons. Instructions for completing these lessons start at https://www.freecodecamp.org/learn/quality-assurance/quality-assurance-and-testing-with-chai/

## Basic Assertions

1.  ### Learn How JavaScript Assertions Work
    Within tests/1_unit-tests.js under the test labelled #1 in the Basic 
    Assertions suite, change each assert to either assert.isNull or 
    assert.isNotNull to make the test pass (should evaluate to true). Do not 
    alter the arguments passed to the asserts.

2. ### Test if a Variable or Function is Defined
   Within tests/1_unit-tests.js under the test labelled #2 in the Basic 
   Assertions suite, change each assert to either assert.isDefined() or 
   assert.isUndefined() to make the test pass (should evaluate to true). Do 
   not alter the arguments passed to the asserts.

3. ### Use Assert.isOK and Assert.isNotOK
   isOk() will test for a truthy value, and isNotOk() will test for a falsy 
   value.
   Within tests/1_unit-tests.js under the test labelled #3 in the Basic 
   Assertions suite, change each assert to either assert.isOk() or 
   assert.isNotOk() to make the test pass (should evaluate to true). Do not 
   alter the arguments passed to the asserts.

4. ### Test for Truthiness
   isTrue() will test for the boolean value true and isNotTrue() will pass 
   when given anything but the boolean value of true.

   assert.isTrue(true, 'This will pass with the boolean value true');
   assert.isTrue('true', 'This will NOT pass with the string value "true"');
   assert.isTrue(1, 'This will NOT pass with the number value 1');

   Within tests/1_unit-tests.js under the test labelled #4 in the Basic 
   Assertions suite, change each assert to either assert.isTrue or 
   assert.isNotTrue to make the test pass (should evaluate to true). Do not 
   alter the arguments passed to the asserts.

## Equality

1. ### Use the Double Equals to Assert Equality
   equal() compares objects using ==.

   Within tests/1_unit-tests.js under the test labelled #5 in the Equality 
   suite, change each assert to either assert.equal or assert.notEqual to 
   make the test pass (should evaluate to true). Do not alter the arguments 
   passed to the asserts.

2. ### Use the Triple Equals to Assert Strict Equality
   strictEqual() compares objects using ===.

   Within tests/1_unit-tests.js under the test labelled #6 in the Equality 
   suite, change each assert to either assert.strictEqual or 
   assert.notStrictEqual to make the test pass (should evaluate to true). Do 
   not alter the arguments passed to the asserts.

3. ### Assert Deep Equality with .deepEqual and .notDeepEqual
   deepEqual() asserts that two objects are deep equal.

   Within tests/1_unit-tests.js under the test labelled #7 in the Equality 
   suite, change each assert to either assert.deepEqual or 
   assert.notDeepEqual to make the test pass (should evaluate to true). Do 
   not alter the arguments passed to the asserts.