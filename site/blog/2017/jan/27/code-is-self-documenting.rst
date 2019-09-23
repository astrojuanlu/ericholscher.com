.. post:: Jan 27, 2017
   :tags: self-documenting, docs, developers, software

"My Code is Self-Documenting"
=============================

Self-documenting code is one of the biggest documentation myths in the software industry.
This view generally conflates documentation with code comments.
I'd like to make two arguments in this post:

* Code comments have value
* Documentation has more value than just explaining how software works

Code comments have value
------------------------

Generally the argument for "self-documenting code" boils down to:

* I can make small objects/functions that have one specific use
* That specific use will be represented in its name
* I don't need to explain anything else because now it's obvious how this program works

**Code comments document the why, not the how.**
They are important to transfer knowledge to both people reading the code or developers working on the code.

Some common uses of comments:

* Explaining previous approaches that didn't work
* Presenting an example usage of the function and example output
* Explaining trade offs in the current implementation
* Marking possible improvements (TODOs) in the code
* Anything else you'd like to communicate with someone reading or developing the code

**Object names document the how, not the why.**
They are effectively inverses of each other.
An argument against comments is an argument against communication.
It's effectively saying *"anyone who needs to know how to use a piece of code is best served by reading that code"*.
This is true for a vanishingly small amount of software users.

Once you start writing quality code comments,
you can use a tool like Sphinx or Javadoc to include them in your documentation.
This allows you to include your up-to-date code comments in your guides and references.
Making use of your code comments this way adds incentive to keep them up to date,
since they will be shown to your users.

Documentation is more than code comments
----------------------------------------

The other fatal flaw of the "self-documenting code" mindset is that it is myopic.
It takes a developer-only point of view,
only seeing the value of documentation as allowing people to understand how code works.
**Documentation is for every possible user.**

I have a few rhetorical questions about this philosophy:

* Where does the tutorial go in your self-documenting code?
* How do you put installation instructions in your variable names?
* What do the answers to questions from your users go in the code?

Developers only thinking about developers when they are working on software is a problem.
A vast majority of software users are not people who develop that software.
**Saying that variable names are the only documentation needed means that only people who read your code can use it**.

One of my goals in the world is to make software more usable.
Having good documentation makes software approachable and usable by people who aren't developers.
People who believe in a world of self-documenting code are making it harder for normal people to use our software.

If you want to have users for the software you write,
you have to write documentation.
