repo
====

*Make any VCS speak a common tongue*

While the OSS community converges to Git,
with the Python bunch branching to Mercurial,
the typical workplace is stuck with Subversion...
And my DVCS of choice is Fossil.

These are all fine projects,
with their own pros and cons,
but what you usually want is just a tool 
to store your code tree snapshot in a safe place.
They can all do that, but their language differs a tiny bit.
Why think if you need to push manually,
or was it *log* or *history* or *timeline*?
Heck, why even bother with remembering which one are you using right now?

Unified language
----------------

This script brings them all down to the common root.
It works by detecting which VCS are you using right now
and calling that,
applying necessary subcommand translation if needed.

There are four basic operations you normally need:

- *repo commit* - commits (-a in Git) and pushes if necessary

- *repo up* - updates your tree, pulling if necessary

- *repo diff* - shows the changes between current and repository trees

- *repo log* - shows the history of changes

Notably, there is no *revert* in that list.
That's because you actually should think before reverting...

Installation
------------

Just take the *repo* script from this repository 
and put it somewhere in your path.
Have fun.

Protip
------

This can be used to great effect 
to get one-click repository integration into Vim :)
