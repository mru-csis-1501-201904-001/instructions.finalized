# Design Guidelines

- [ ] read the assignment instructions (including notes) carefully; ignoring instructions is a Bad Idea
- [ ] you should deliver the software you were asked to deliver - don't add extra features that aren't asked for

---

- [ ] choose your constant, variable, method, and parameter names carefully - they should be easy to understand, descriptive, and never lie
- [ ] put all your constant declarations at the top of your code using **private static final**
- [ ] whenever possible, declare variables at first use
- [ ] choose variable types that fit their purpose
- [ ] replace magic numbers that have **meaning** with well-named constants; if you can't find a good name, it's probably not a magic number you need to replace!

---

- [ ] keep your methods short - anything more than 20 lines and I'm gonna start getting cranky! Prefer lots of small, well-focused methods over larger globs.
- [ ] likewise, keep your parameter lists short - in general, anything over 3 is highly suspect. Prefer methods that have 0 or 1 argument. 2 is OK. 3 is pushing it.

---

- [ ] you should briefly document things that aren't obvious and/or that come from external sources (a brief note and a URL is fine)
- [ ] you don't need to comment code that already speaks for itself

---

- [ ] strive for the ideal of "clean code":
  - "Clean code is simple and direct. Clean code reads like well-written prose." [Grady Booch]
  - "You know you are working with clean code when [it]... turns out to be pretty much what you expected." [Ward Cunningham]
- [ ] all else being equal, it is better to be expressive than clever
- [ ] remove code that doesn't do anything
- [ ] keep an eye out for duplicate code; use well-named helper methods to capture the duplication in one place
- [ ] capture complex code (steps, or even complex conditionals) in well-named helper methods

---

- [ ] use whitespace to improve readability, both within statements and between statements
- [ ] don't use (x == true) or (x == false) in your code
- [ ] be consistent: don't mix bracing styles, indentation, incrementation methods, etc.

---

- [ ] create prompts that are easy to understand by the end-user
