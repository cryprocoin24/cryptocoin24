Cryptocoin24 integration/staging tree
================================

http://www.cryptocoin24.org

Copyright (c) 2009-2014 Bitcoin Developers
Copyright (c) 2011-2014 Cryptocoin24 Developers

What is Cryptocoin24?
----------------

CRC24 is short for Cryptocoin 24. CRC24 is a cryptocurrency, much like Bitcoin. Here is the original whitepaper.
The concept behind Cryptocoin24 is very innovative, as there will be no tokens or blocking periods for Cryptocoin24 owners. A Coin which not only stands out from others, but is revolutionary.
Cryptocoin24 is designed not only for insiders of cryptographic technologies, but is intended to be easily usable and usable by all people worldwide. Its potential is enormous because it is to be recognized as a separate means of payment and this is completely independent of banks.

For more information, as well as an immediately useable, binary version of
the Cryptocoin24 client sofware, see https://www.cryptocoin24.org.

License
-------

Cryptocoin24 is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Cryptocoin24
development team members simply pulls it.

If it is a *more complicated or potentially controversial* change, then the patch
submitter will be asked to start a discussion with the devs and community.

The patch will be accepted if there is broad consensus that it is a good thing.
Developers should expect to rework and resubmit patches if the code doesn't
match the project's coding conventions (see `doc/coding.txt`) or are
controversial.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/cryptocoin24-project/cryptocoin24/tags) are created
regularly to indicate new official, stable release versions of Cryptocoin24.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test. Please be patient and help out, and
remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write unit tests for new code, and to
submit new unit tests for old code.

Unit tests for the core code are in `src/test/`. To compile and run them:

    cd src; make -f makefile.unix test

Unit tests for the GUI code are in `src/qt/test/`. To compile and run them:

    qmake BITCOIN_QT_TEST=1 -o Makefile.test bitcoin-qt.pro
    make -f Makefile.test
    ./cryptocoin24-qt_test

