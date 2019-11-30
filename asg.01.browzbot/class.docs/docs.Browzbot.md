# Browzbot Notes

## Preamble

This is a class you need to _complete_. Make sure you read any comments present in its source file.

Although BrowserAutomationApp is the "manager" of the assignment, Browzbot is the workhorse who actually does most of the heavy lifting.

If a Browzbot object (which I'll sometimes just call a "bot") is created via `new Browzbot("chrome")`, a Chrome browser window will open. If created any other way, no browser will open.

Once a Browzbot object is created, it can be told to do just one thing: "run" an instruction.

Bots understand the following instructions:

- STOP
  - closes the browser currently being driven by the bot
- BACK
  - activates the "Back" button on the browser
- FORWARD
  - activates the "Forward" button on the browser
- OPEN [website]
  - attempts to open the given website in the browser
- SHOOT [screenshot name]
  - takes a screenshot of the current webpage and assigns it the given name; this image will be saved in the Eclipse project directory
- WAIT [number of seconds]
  - the bot will wait the given number of seconds; this is useful for giving the browser time to load a page fully
- CLICK [type of click][thing to click]
  - causes the browser to click something; if [type of click] is:
    - ID, then a web page element with the id = [thing to click] is clicked
    - CLASS, then a web page element with a class = [thing to click] is clicked
    - LINK, then a link with the text [thing to click] is clicked
- FILL [id][text]
  - the form field with the given id is filled with the given text
- SELECT [id][dropdown text]
  - selects a dropdown item from a dropdown with the given id

### About IDs, CLASSes, LINKs, FORMs, and DROPDOWNs

Unless you've done some web design in the past, these things won't make much sense. Since this is not a web design course (that's COMP1511!), JP will put out a screencast about how to find these things in an actual web page. You'll be notified when this screencast is available and where to find it.

## Public Methods You **Must** Make

1. **run**

## Private Methods You **Must** Complete

1. **handle**

## Helper Methods

Trying to put all the code necessary to make `run` work IN `run` will be pretty damn ugly. You will want to make some private helper methods to make your `run` easier to read and understand.

## Testing

To confirm your Browzbot class is working as expected, you want all these tests to pass:

- `BrowzbotRunsInstructionSuccessfullyTests`
- `BrowzbotRunsInstructionWithWrongNumberOfArgsTests`
- `BrowzbotRunsUnknownInstructionTests`

None of the above tests will actually open a browser; they're just making sure that the Result coming back is as expected. This is done to keep the time required to run the tests down.

