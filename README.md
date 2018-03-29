Innoket Core integration/staging tree
=====================================

[![Build Status](https://travis-ci.org/innoket/innoket.svg?branch=master)](https://travis-ci.org/innoket/innoket)

https://innoket.io

What is Innoket?
----------------

Innoket is a marketplace where idea, subjects, topics, articles and
opinions is our priority. The idea behind this system is pretty simple. Most
of the problems faced by many investors are the unavailability of the
right field and scheme to put investments in. The fund is available for
investment but no idea on what to invest in which made us to come up
with this idea marketplace which gives many investors a very wide range
of business opportunities to invest into to yield massive profits


For more information, as well as an immediately useable, binary version of
the Innoket Core software, see https://innoket.io/en/download, or read the
[original whitepaper](https://www.innoket.io/content/Innoket%20Whitepaper.pdf).

License
-------

Innoket Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/innoket-dev/innoket-master/tags) are created
regularly to indicate new official, stable release versions of Innoket Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](src/test/README.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`. Further details on running
and extending unit tests can be found in [/src/test/README.md](/src/test/README.md).

There are also [regression and integration tests](/test), written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/test) are installed) with: `test/functional/test_runner.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.
