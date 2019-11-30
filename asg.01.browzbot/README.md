# Assignment 01

**DUE:** Friday, October 18, 2019 @ 11:59PM

**LATE SUBMISSION DEADLINE:** Friday, December 6, 2019 @ 11:59PM

You may submit this assignment late, without penalty, up to the given deadline.

**WEIGHT:** 5%

## SUBMISSION PROCEDURE

To submit your assignment, submit your entire `src` directory just as you would for a lab quiz.

## If you have QUESTIONS

If you've looked through the instructions and cannot find an answer, please feel free to post a question [to this Google Doc](https://docs.google.com/document/d/1kIocWkbE6nxEW2GJmPyrOLYkyxBmg_R5ZuvvBVCnu8U/edit?usp=sharing) - I'll be monitoring it frequently.

## A suggested PLAN OF ATTACK

1. read all of this Readme
1. read [the assignment overview doc](asg.01.browZbot.docs.md); it tells you what this assignment is about and shows you how the software you are going to build looks and behaves
1. glance through the [list of classes used](list.of.classes.used.md) for the 7 different classes that are involved in the software you are building - this list will give you a feel for how all the pieces of the application work together and also give you an idea at which classes will be harder to complete than others
1. cherry-pick a non-threatening class and get it passing its tests. Don't forget to make sure you're keeping on top of any problems being reported by Checkstyle, PMD, and Spotbugs as well - **don't** put those problems off for later, because they'll become a very discouragingly-sized mountain which you'll likely just ignore when you're all exhausted at the end of this assignment.
1. keep up this process - once all tests are green, you should have a working application! Submit that puppy!

## A few WARNINGS

- For most of you, this is your first programming assignment. Programming assignments will _always_ take longer than you think. Because you **will** get stuck in places, if you try and do this assignment a day or two before it's due, your life will be a grey and dismal thing.
- You might be dismayed at the amount of text in the instructions and documentation. It's there for a reason. _Skim at your peril._
- The information you need to complete this assignment will be scattered about in a variety of places: in these instruction files, in the code documentation, in the Google Doc mentioned above in the "If you have QUESTIONS" section, and in the code itself. This mimics real-life projects, where there is rarely one definitive "source of truth." As you're working through the resources you've been given, take notes - keep track of things that you suspect will be useful.

## Getting the starting code

The starting code is obtained just like it would be for a lab quiz: through GitHub Classroom.

Here's the link: <https://classroom.github.com/a/RsPpJNUK>

## How to check your work

If you want to check whether your code is _behaving as expected_, you should run any (and eventually all!) of the tests in the test directory.

If you want to see whether your code is _following the coding standards for this course_, you should see if you are receiving any errors or warnings from any of Checkstyle, PMD, or Spotbugs in the Problems View.

> There is some overlap between the tools used to do style checking, so
> you may notice some warnings are repeated between the three tools. If you
> don't understand any of the warnings (they **can** be a little opaque), please check the properties of the problem first - if you're still unclear what's going on, it's time to talk to one of the IAs or your instructor.
