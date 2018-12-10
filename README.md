# Feed Reader Testing

Feed Reader Testing, is a project that mainly trains a developer to know how a testing of a project in real world is done.
Testing can also be known as Red-Green-Refactor, where you write code which fails first and then you debug and make it green.

In this Testing Jasmine-2.1.2[] is used as a tester.

# Running this application
   To run this application clone the repository ⏬
   ```
   $ git clone https://github.com/sb39/FeedReader-project.git
   ``` 
   open `index.html` file 
   
#important components covered

1. Red-Green-refactoring 
    a. test suites(`describe` calls):
        A test suite begins with a call to the global Jasmine function `describe` with two parameters: a string and a function. 
        **The string is a name or title for a spec suite - usually what is being tested.**

    b. specs(`it` calls):
        Specs are defined by calling the global Jasmine function `it`, which, like describe takes a string and a function.
        **A spec contains one or more expectations that test the state of the code.**
2. `beforeEach` Calls:
    there are some code components which needs to be called again and again in the `spec` component. It feels convenient to call them 
    again and again, but for long and complex code, *it may make code look more complex*. 
    *syntax*
    ```
    beforeEach(function(paramenter){
        // block of code
    });
    ```
3. Asynchronous calls
    some assertions in despite of having functions to set their actual timeout, are executed before the actual change takes place.
    So, testing promises or AJAX calls may result in the same fate.
    The `done()` method:
        done is a function in jasmine which actually waits for the function to execute before moving forward.
        `The default timeout of the done() function is 5secs`.

# Code dependencies 
1. [Icon Font & SVG Icon Sets ❍ IcoMoon](https://icomoon.io/)
2. [Normalize.css](https://necolas.github.io/normalize.css/)
3. [Google Fonts](https://fonts.google.com/)
4. [JasmineJS](https://jasmine.github.io/)
5. [HandlebarJS](https://handlebarsjs.com/)
6. [jQuery](https://jquery.com/)
7. [Google's loading API](https://www.google.com/jsapi)


