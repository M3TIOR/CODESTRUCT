# Darklight Repository Structure

This repository is meant to be a semi-interactive brief on the programming
structure our source will be taking across multiple repo's.

The aim here is to provide a directory structure that can be seamlessly
integrated with and abstracted upon. This is by no means an easy task when
you factor in every possible language we have to support. And since every day
there is the possibility of a new language arising, we have to use a system
that is open-ended.

### Directory Structure:
 1. [bin](./bin/README.md)
   * (platform)
 * [doc](./doc/README.md)
 * [include](./include/README.md)
   * (distributor)
     * (repository/program name)
 * [res](./res/README.md)
 * [src](./src/README.md)
 * [tools](./tools/README.md)
   * (distributor)
     * (tool name)

The current directory tree you see before you is exactly what we have
put together to accomplish this task. It's capable of supporting the include
feature, which allows programs to call out to other [API]'s and the like.
Without such a feature, code would be excessively redundant. All programs that
aren't managed in [virtual machines][VM] or scripting environments would need to
do things that would be otherwise unnecessary, and similar can be said for
their [VM] and script counterparts; who rely upon the built-ins that their parent
binaries support. When an [interpreter] or [VM] doesn't support what a program built
within it needs, that program then needs to outsource or build in their own
solution to a problem.

Repositories also need documentation; especially useful information
to users when you have an extensive tool that you want to distribute to a large
audience. Or, in the case of games and such, documentation can simply be a way
for ideas to be fleshed out, lore to be expanded upon, etc. It's most valuable
property though, is that documentation lays the ground-work for how it's
corresponding program behave. **In most cases, a program should be documented
far before programming begins.** This ensures that anyone using the program
can also debug it to some degree, along with being able to accurately use it.
It also makes things easier for the programmers because then they don't have to
think of how the program is to function themselves and they can focus primarily
on the best ways to optimize that programs performance. *The exception being
when the programmer is also the program-architect.* That does not exclude their
code from needing proper documentation however.

Sometimes it's useful to include tools for building a repository with it. It's
a common trend that you will see with large projects to include shell scripts
and other related build tools with a repository as a means of ensuring that
their product can be built and used on any platform.

And of course we all know that no repository is complete without it's source
code.

By using this organization structure you support all that and more. Along with
all our code as well.

To learn what each folder is meant to store and it's use, click on it's
corresponding link in this list. Or if you're viewing this on github, you can
alternatively click the folders readme in the file browser. ***cause, ya' know,
that's exactly what the above links will redirect you to anyway.***

[VM]: https://en.wikipedia.org/wiki/Virtual_machine
[interpreter]: https://en.wikipedia.org/wiki/Interpreter_(computing)
[API]: https://en.wikipedia.org/wiki/Application_programming_interface
