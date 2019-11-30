# List of Classes Used

Here's a list of all the classes involved in this assignment. It looks like a lot, but before you hyperventilate, three things:

1. two of the classes are already complete and you don't have to code them up!
1. three more classes are already _partially_ complete, so you will only need to add some code to them - but you **will** need to look through the code that's already there to help you complete them properly. This "reading other people's code" thing is a **good** thing, because it's something that developers do - a **lot** - and the more practice you get with it, the better. So start eating your veggies.
1. having numerous classes like this is very common in object-oriented programming - we create classes that have a specific job in life, and by doing so, we often wind up with a lot of classes. Fortunately, since these classes (should be) small and focused, they are easier to write and to understand.

## Completed Classes (2)

These are classes that are fully complete - you can read through them if you wish, but you should not alter them in any way.

1. Main
1. NullWebDriver

## Classes You Must Complete On Your Own (2)

These are classes that you need to create from scratch. **They must follow the public interface used in their corresponding tests**; if they don't, significant mark reduction will occur. That's because if you deviate from the required public interface, the automated tests won't work on your code and so I gotta roll up my sleeves and manually try to figure out what you're doing and then I'll start to get grumpy and then things end poorly for both of us.

I've tried to indicate how easy I think each class is to code (☆ = easiest, ☆☆☆ = hardest). I have also given the dependencies for the class - that is, what classes you need to complete before you can work on the given class.

These all hyperlink to a document with some notes on each class:

1. [Result](class.docs/docs.Result.md) ☆
   - no dependencies
1. [Instruction](class.docs/docs.Instruction.md) ☆☆
   - no dependencies

## Partially Completed Classes (3)

These are classes that are _partially_ completed; there are some methods that you will need to create to make the class work properly. Each of these methods is marked with a TODO comment.

> **Pro Tip**
>
> _In Eclipse, you can see a list of these TODOs by going `Window → Show View → Tasks` (**not** TaskList!)_

I've tried to indicate how easy I think each class is to code (☆ = easiest, ☆☆☆ = hardest). I could be way off.

These all hyperlink to a document with some notes on each class:

1. [Browzbot](class.docs/docs.Browzbot.md) ☆☆☆
   - depends on `Result`
   - depends on `Instruction`
1. [UserInterface](class.docs/docs.UserInterface.md) ☆
   - no dependencies (that you have to worry 'bout)
1. [BrowserAutomationApp](class.docs/docs.BrowserAutomationApp.md) ☆☆½
   - depends on `Browzbot`
   - depends on `UserInterface`
