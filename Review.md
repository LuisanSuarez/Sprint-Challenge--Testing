# Please answer the following questions

1.  In Jest, what are the differences between `describe()` and `it()` globals, and what are good uses for them?
Describe creates a test Suite. It doesn't actually run any tests itself, but it
groups different tests into a 'Suite'. It helps organize different test into similar categories.
'It' actually runs the test.

2.  What is the point of `Test Driven Development`? What do you think about this approach?
To ensure that the code is working robustly from the ground up. Because you're writing the code to pass any requirements you're testing from the ground up, you can be sure that every time you refactor your code you'll be sure whether or not it'll behave like you want it to.
I think it's great for functionalities that are either a)complex, b)vital/central or both. For other simpler, more frequent, and easy-to-fix functionalities I think that the upfront cost of TDD is too high. I would rather write the tests after the fact to make sure it doesn't break, but if I'm very familiar with what the function is going to do I think it's too much effort and time.

3.  What are `mocks`? What are a good use cases for them?
Mocks are methods or objects that simulate behavior that my functions will respond to (e.g. a response from an API after it's called).
It's great when my application is going to interact with outside resources that are out of my control. I can intentionally set the mock to fail and to pass to test for both scenarios (rather than hoping that the API fails so I can see how my application handles it, or waiting for it to work if the server happens to be down that day. )

4.  Mention three types of automated tests.
Unit, Integration, Snapshot
Unit - a single, isolated functionality
Integration - various components working together
Snapshot - a JSON rendering and comparison of the UI generated by the code.
