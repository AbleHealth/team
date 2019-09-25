# Engineering Team Mission, Principles, and Practices

This document is not written in stone, but it is important in that it is our
agreement with one another. This is a living document, intended to guide us in
the spirit and the methods of our work. As we work and discover what works for
us as a unique team, and what does not, this document should be modified or
appended to.  

Feel free, at any time, to submit a merge request or propose a meeting. Merge
requests specifically to this document should be agreed upon by everyone. If
meeting with the group and everyone says 'yea' to a change, it can simply be merged in.

As an engineering team, we seek to:

- Build an [esprit de corps](https://www.dictionary.com/browse/esprit-de-corps) where the engineering team is inspired to ship high quality software on a predictable schedule
- Create a culture of trust where engineers feel they have the freedom to do great work, share vulnerabilities, and inquire
- Create a culture of inclusion where all engineers feel they have a voice
- Create a culture of ownership where engineers take responsibility for shipping high quality code, system performance & uptime, and client happiness
- Foster an environment where engineers are challenged, strive for excellence and continually improve
- Encourage a culture of self-organizing teams

## Our Mission
__Our mission is more than writing software.__

Our mission in engineering is two-fold:

* **Build and deliver the Able Platform** into the hands of our customers
* **Seek out ways to make the working lives of our colleagues simpler, more pleasant, and more productive**

## Able Engineering Principles
- Do the work
- Don’t let perfect be the enemy of perfectly good
- Strive for simplicity
- Insist on extreme visibility
- Trust and empower
- Embrace change

## Practices
### Ship working software often

We use the practice of continuous integration (CI) where we're frequently merging code into our mainline branch, `master` - often multiple times a day. A set of automated tests with very high code coverage (100%) provide assurance that no regressions are introduced. If the tests fail, the team stops what they are doing to fix the problem immediately.

1. All branches pushed to GitHub will be run in CI. When you break the build, it’s up to you (and/or your partner) to fix it.
2. When master passes CI, it is deployed immediately to a publicly available server.

You can read more about our CI process [here](https://docs.google.com/document/d/1m-u-6LRPjPisBuESP0rkIxJrNiMObovvsRbszwsdNLc/edit)

### Short iterations
We work in short, 1-week milestones (an "iteration"). The goal of each milestone build is to show progress (which keeps us honest) and to deliver it with a high enough level of quality that our community can really use it and provide feedback (which keeps us even more honest).

### Get multiple eyes on code before shipping
In keeping with `insisting on extreme visibility` and `trust and empower` we seek to collaborate on design and review code through:
- Design sessions, which are best when multiple perspectives and team alignment on the approach to a project or story are helpful
- Pair programming, which is best when the domain is new, errors are likely or costly, or team members are unfamiliar with the portion of the codebase
- Pull requests, which are required when code is not paired on to ensure quality and maintainability of code
If pull request comments include major architectural feedback, this is an indication that more work to collaborate and align the team would have been helpful in advance of delivering the code.

### Tests are more important than code
- Tests give us confidence that any change we make doesn’t break something else, even if it’s "unrelated"
- The sooner you find a bug, the cheaper and easier it is to fix it.
- A test suite that takes a long time is one that will be used much less often. The entire test suite should take less than five minutes to build on a developer’s laptop.
- Try to write tests before the code. Write one failing test, make it work, and then write the next failing test. Getting the first test to work often informs writing of the second. If you write tests based on unvalidated assumptions, you’ll have to modify them all when the assumptions turn out to be wrong. System-level tests give you a sense of certainty that the whole system is working.
- Every commit to master should pass all tests.

### Design is part of everyone's daily business
- Use incremental design instead of creating one big design at the beginning of a project. Take small, safe steps and test your designs.
- Duplication is a sign that design needs to be reconsidered.
- Refactor mercilessly and with focus.
  - :white_check_mark: Refactor code that is in the direct line of your code path
  - :white_check_mark: Refactor code that makes the delivering feature in progress ultimately much easier
  - :interrobang: Bias against refactoring code that's not directly involved in the work at hand
  - **It's a balance**: Look for opportunities to leave code you work in better condition than you found it, but remember the overarching principle of "Don’t let perfect be the enemy of perfectly good."

### Apply the simplest thing that will work
- Keep software designs simple. Build small, self-contained units: classes, modules, services, etc. They should do only one thing; this helps avoid changes that require shotgun surgery.
- YAGNI: You Aren’t Going To Need It. Build features that are defined right now in stories; do not build features you think will be needed in the future.
- Delete unnecessary/duplicative code. The most destructive thing you can do to your project is to build new code, and then build more code that depends on it, and then still more code that depends on that, leading to that painfully familiar domino effect of cascading changes... and eventually leaving you with an unmaintainable mess of spaghetti code. Delete code and run the tests.
