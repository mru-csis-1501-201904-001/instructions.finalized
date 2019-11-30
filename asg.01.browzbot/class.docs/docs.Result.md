# Result Notes

## Preamble

This is a class you need to _create_.

Its job in life is to represent the result of a Browzbot object running an instruction. The result needs to store a numeric exit code and a message (which briefly describing what the exit code actually means in English).

It's very short. Like less than 20 lines of code short.

## Suggestions

If you want to see examples of Result objects returned by a Browzbot object running an instruction, check out the tests that start with **BrowzbotRuns** (like `BrowzbotRunsInstructionSuccessfullyTests` and `BrowzbotRunsInstructionWithWrongNumberOfArgsTests`).

## Public Methods You Need To Make

You can figure out all required public methods you will need by looking at the single test in `ResultSimpleTests`.

## Testing

You want all the tests in the following class to pass:

- `ResultSimpleTests`
