# Instruction Notes

## Preamble

This is a class you need to _create_.

Its job in life is to represent an instruction typed in by a user at the console; this instruction is meant to be run by a Browzbot object.

Each instruction object is created from a String. Each String is composed of 0 or more **tokens** separated by whitespace (either spaces or tabs):

- `"look over there"` has three tokens: "look", "over", and "there"
- `"what?"` has one token: "what?"
- `" oh crud "` has two tokens: "oh" and "crud" (leading and trailing whitespace is removed!)
- `""` (the empty string) has zero tokens

Each instruction is composed of a **command** and 0 or 2 **arguments**:

- `"stop"` has one command (**STOP**) and 0 arguments
- `"open imdb.com"` has one command (**OPEN**) and 1 argument (**imdb.com**)
- `"click id search"` has one command (**CLICK**) and 2 arguments (**id** and **search**)
- `"click link onward to victory, friends!"` has one command (**CLICK**) and 2 arguments (**link** and **onward to victory, friends!**)

## Suggestions

- Read through the tests that start with **Instruction** (like `InstructionCreationFromMoreThanThreeTokensTests` and `InstructionRemovalOfExtraWhitespaceInArgumentTwoTests`) to understand more fully how an instruction is supposed to behave.
- Almost all of the work in this class is done in the constructor; it would be a good idea to use private helper methods to make your constructor code more readable. (Many beginning programmers are surprised to hear they can use helpers in constructors...but a constructor is just a method - albeit a little bit weird-lookin').
- `Scanner` works with Strings, not just `System.in`! So you can go
  ```java
  Scanner textScanner = new Scanner("some text 2 scan");
  String word = textScanner.next(); // word is now "some"
  word = textScanner.next(); // word is now "text"
  int num = textScanner.next(); // num is 2
  word = textScanner.next(); // word is now "scan"
  ```
  Crazy useful!
- Scanner has a method called `hasNext()` that you should look up; it will be useful
- Speaking of useful:
  - look up what the String method `trim()` does, and
  - <https://programming.guide/java/removing-duplicate-whitespace.html>

## Public Methods You **Must** Make

I won't provide a list of public methods for you to make; instead, I'd like you to practice reading code that involves a class to determine the public interface of the class!

_Translation: go through the InstructionBlahBlah tests and note what methods are called on Instruction objects by the tests - those are the methods you need to create! Here's an example:_

```java
// in the InstructionCreationFromOneTokenTests.java file
assertThat(instruction.argumentOne()).isEqualTo("");

// since instruction is an Instruction object, we can instantly
// see that the Instruction class has a public method
// called argumentOne() that returns a String!
```

## Testing

You want all the tests in the following classes to pass:

- `InstructionCreationFromMoreThanThreeTokensTests`
- `InstructionCreationFromThreeTokensTests`
- `InstructionCreationFromTwoTokensTests`
- `InstructionCreationFromOneTokenTests`
- `InstructionCreationFromZeroTokensTests`
- `InstructionRemovalOfExtraWhitespaceInArgumentTwoTests`
