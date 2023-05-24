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

## Comparison

1. ### Compare the Properties of Two Elements
    Within tests/1_unit-tests.js under the test labelled #8 in the 
    Comparisons suite, change each assert to either assert.isAbove or 
    assert.isAtMost to make the test pass (should evaluate to true). Do not 
    alter the arguments passed to the asserts.

2. ### Test if One Value is Below or At Least as Large as Another
   Within tests/1_unit-tests.js under the test labelled #9 in the Comparisons 
   suite, change each assert to either assert.isBelow or assert.isAtLeast to 
   make the test pass (should evaluate to true). Do not alter the arguments 
   passed to the asserts.

3. ### Test if a Value Falls within a Specific Range
   Within tests/1_unit-tests.js under the test labelled #10 in the 
   Comparisons suite, change each assert to assert.approximately to make the 
   test pass (should evaluate to true).

  Choose the minimum range (3rd parameter) to make the test always pass. It 
  should be less than 1.

  ## ARRAY
  
  1. ### Test if a Value is an Array
     As a reminder, this project is being built upon the following starter 
     project on Replit, or cloned from GitHub.

    Within tests/1_unit-tests.js under the test labelled #11 in the Arrays 
    suite, change each assert to either assert.isArray or assert.isNotArray to 
    make the test pass (should evaluate to true). Do not alter the arguments 
    passed to the asserts.

2. ### Test if an Array Contains an Item
   As a reminder, this project is being built upon the following starter 
   project on Replit, or cloned from GitHub.

   Within tests/1_unit-tests.js under the test labelled #12 in the Arrays 
   suite, change each assert to either assert.include or assert.notInclude 
   to make the test pass (should evaluate to true). Do not alter the 
   arguments passed to the asserts.

   ## STRINGS

   1. ### Test if a Value is a String
   As a reminder, this project is being built upon the following starter 
   project on Replit, or cloned from GitHub.

  isString or isNotString asserts that the actual value is a string.

  Within tests/1_unit-tests.js under the test labelled #13 in the Strings 
  suite, change each assert to either assert.isString or assert.isNotString 
  to make the test pass (should evaluate to true). Do not alter the 
  arguments passed to the asserts.

  2. ### Test if a String Contains a Substring
As a reminder, this project is being built upon the following starter project on Replit, or cloned from GitHub.

include() and notInclude() work for strings too! include() asserts that the actual string contains the expected substring.

Within tests/1_unit-tests.js under the test labelled #14 in the Strings suite, change each assert to either assert.include or assert.notInclude to make the test pass (should evaluate to true). Do not alter the arguments passed to the asserts.

3. ### Use Regular Expressions to Test a String
As a reminder, this project is being built upon the following starter project on Replit, or cloned from GitHub.

match() asserts that the actual value matches the second argument regular expression.

Within tests/1_unit-tests.js under the test labelled #15 in the Strings suite, change each assert to either assert.match or assert.notMatch to make the test pass (should evaluate to true). Do not alter the arguments passed to the asserts.

### Object

1. ### Test if an Object has a Property
As a reminder, this project is being built upon the following starter project on Replit, or cloned from GitHub.

property asserts that the actual object has a given property.

Within tests/1_unit-tests.js under the test labelled #16 in the Objects suite, change each assert to either assert.property or assert.notProperty to make the test pass (should evaluate to true). Do not alter the arguments passed to the asserts.





# FUNCTIONAL TEST

## Integration test with chai-HTTP

1. Run Functional Tests on API Endpoints using Chai-HTTP
As a reminder, this project is being built upon the following starter project on Replit, or cloned from GitHub.

Mocha allows you to test asynchronous operations like calls to API endpoints with a plugin called chai-http.

The following is an example of a test using chai-http for a suite called 'GET /hello?name=[name] => "hello [name]"':

suite('GET /hello?name=[name] => "hello [name]"', function () {
  test('?name=John', function (done) {
    chai
      .request(server)
      .keepOpen()
      .get('/hello?name=John')
      .end(function (err, res) {
        assert.equal(res.status, 200, 'Response status should be 200');
        assert.equal(res.text, 'hello John', 'Response should be "hello John"');
        done();
      });
  });
});
The test sends a GET request to the server with a name as a URL query string (?name=John). In the end method's callback function, the response object (res) is received and contains the status property.

The first assert.equal checks if the status is equal to 200. The second assert.equal checks that the response string (res.text) is equal to "hello John".

Also, notice the done parameter in the test's callback function. Calling it without an argument at the end of a test is necessary to signal that the asynchronous operation is complete.

Finally, note the keepOpen method just after the request method. Normally you would run your tests from the command line, or as part of an automated integration process, and you could let chai-http start and stop your server automatically.

However, the tests that run when you submit the link to your project require your server to be up, so you need to use the keepOpen method to prevent chai-http from stopping your server.

Within tests/2_functional-tests.js, alter the 'Test GET /hello with no name' test (// #1) to assert the status and the text of the response to make the test pass. Do not alter the arguments passed to the asserts.

There should be no URL query. Without a name URL query, the endpoint responds with hello Guest.

2. ### Run Functional Tests on API Endpoints using Chai-HTTP II
As a reminder, this project is being built upon the following starter project on Replit, or cloned from GitHub.

Within tests/2_functional-tests.js, alter the 'Test GET /hello with your name' test (// #2) to assert the status and the text of the response to make the test pass.

Send your name as a URL query by appending ?name=<your_name> to the route. The endpoint responds with 'hello <your_name>'.

3. ### Run Functional Tests on an API Response using Chai-HTTP III - PUT method
As a reminder, this project is being built upon the following starter project on Replit, or cloned from GitHub.

When you test a PUT request, you'll often send data along with it. The data you include with your PUT request is called the body of the request.

To send a PUT request and a JSON object to the '/travellers' endpoint, you can use chai-http plugin's put and send methods:

chai
  .request(server)
  .keepOpen()
  .put('/travellers')
  .send({
    "surname": [last name of a traveller of the past]
  })
  ...
And the route responds with:

{
  "name": [first name],
  "surname": [last name],
  "dates": [birth - death years]
}
See the server code for the different responses to the '/travellers' endpoint.

Within tests/2_functional-tests.js, alter the 'Send {surname: "Colombo"}' test (// #3) and use the put and send methods to test the '/travellers' endpoint.

Send the following JSON object with your PUT request:

{
  "surname": "Colombo"
}
Check for the following within the request.end callback:

The status should be 200
The type should be application/json
The body.name should be Cristoforo
The body.surname should be Colombo
Follow the assertion order above - we rely on it. Also, be sure to remove assert.fail() once complete.

4. ### Run Functional Tests on an API Response using Chai-HTTP IV - PUT method
As a reminder, this project is being built upon the following starter project on Replit, or cloned from GitHub.

This exercise is similar to the previous one.

Now that you know how to test a PUT request, it's your turn to do it from scratch.

Within tests/2_functional-tests.js, alter the 'Send {surname: "da Verrazzano"}' test (// #4) and use the put and send methods to test the '/travellers' endpoint.

Send the following JSON object with your PUT request:

{
  "surname": "da Verrazzano"
}
Check for the following within the request.end callback:

The status should be 200
The type should be application/json
The body.name should be Giovanni
The body.surname should be da Verrazzano