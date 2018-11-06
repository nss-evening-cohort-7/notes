# Testing
>Speaking of testing, who opted to tackle the [koans](https://github.com/NotMyself/DotNetCoreKoans)? If not, now might be a good time to pick them up.

### Types of Testing
##### Unit testing
The most incremental form of testing and focuses on testing only a single thing. This is often testing a single method, but may depend on your teams definition of what constitutes a "unit".
##### Integration testing
Testing combinations of units and ensuring that they work together properly.
##### System testing
Testing the complete system to ensure that it functions according to the requirements

### Parts of a Test
##### Arrange
Where you setup the initial state of your test. Any classes that need to be instantiated, test data, or parameters will be created here.
##### Act
Where you perform that action that you want to test. Typically this action will give you the result that you are going to test.
##### Assert
Where you're actually performing a test. You can test for lots of things such as equality, method execution, thrown exceptions, etc. You're testing the reality of your action above against your expectations of what should have happened.

### Stages of Testing
##### Red
Write your test. At this stage you won't have written any of the code that you're testing, but you will have "stubbed out" the method so that your code will compile.
##### Green
Write the code that makes your test pass. You will replace the "stubbed out" code in your method(s) with the code that you'll use to solve this single problem. Avoid the temptation to write more code than is absolutely necessary.
##### Refactor
Write the better version of your code. If there's anything that you'd like to clean up about your code this is the time for that. Evaluate if you'd like to refactor the larger solution that might even affect previous tests. Luckily, you have tests to make sure you don't break something.

### Exercises
Roman Numerals
