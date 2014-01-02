Noodlyappendagecoin integration/staging tree
================================

http://www.noodlyappendagecoin.org

Copyright (c) 2009-2013 Bitcoin Developers
Copyright (c) 2011-2013 Litecoinecoin Developers
Copyright (c) 2013-2014 Noodlyappendagecoin Developers

What is Noodlyappendagecoin?
----------------

Noodlyappendagecoin is a lite version of Bitcoin using scrypt as a proof-of-work algorithm.
 - 1 minute block targets
 - Subsidy halves in 525600 blocks (~1 year)
 - ~13.798 billion total coins, one for every year since His Noodly Appendage first touched the universe
 - Difficulty retargets once per hour

For more information, as well as an immediately useable, binary version of
the Noodlyappendagecoin client sofware, see http://www.noodlyappendagecoin.com

License
-------

Noodlyappendagecoin is released under the terms of the MIT license. See `COPYING` for more
information or see http://opensource.org/licenses/MIT.

Development process
-------------------

Developers work in their own trees, then submit pull requests when they think
their feature or bug fix is ready.

If it is a simple/trivial/non-controversial change, then one of the Noodlyappendagecoin
development team members simply pulls it.

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/bitcoin/bitcoin/tags) are created
regularly to indicate new official, stable release versions of Noodlyappendagecoin.

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
    ./noodlyappendagecoin-qt_test

