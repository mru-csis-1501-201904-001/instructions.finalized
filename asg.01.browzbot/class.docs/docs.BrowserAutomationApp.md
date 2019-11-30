# BrowserAutomationApp Notes

## Preamble

This is a class you need to _complete_. Make sure you read any comments present in its source file.

## Suggestions

- the `UserInterface` object passed in to the constructor should handle **all** keyboard input (through the `stringFromUser` method) and **all** console output (via the `print` and `println` methods). This means that BrowserAutomationApp shouldn't do **any** input/output directly itself! (So there shouldn't be a single `System.out` or `System.in` to be seen anywhere!) Any such shenanigans left in your submitted assignment will result in deductions.
- a huge blob of instructions in `run()` is not the way to go: use private helper methods to make your code easy to read - and write
- make your methods short; in my finished code, for example, all methods were under 5 statements long

## Public Methods You **Must** Make

1. **BrowserAutomationApp**
1. **run**

## Public Methods You **Must** Make

1. **userWishesToContinue**
1. **processResponse**

## Testing

Testing of this class is very time-consuming, because you have to spin up a browser and "drive" it...which means that you spend quite a bit of time waiting for things to happen. **Leave testing of this class to the very end of the assignment, after all the other automated tests are running green!**

I will be running a number of automated tests for this class - you can see an example of one such test in the `EndToEndTests` test I've provided you. But there's a catch: I am NOT providing you with the code to ALL of the tests I will be using to test this class.

If you wish to test your code in a similar way - and you should - you'll have run your code and manually provide the proper instructions - or you could look at the code that's given and create your own tests using it as a template....
