SafeMineX Core integration/staging tree
=====================================

[![Build Status](https://travis-ci.org/safeminecoin/safeminex.svg?branch=master)](https://travis-ci.org/safeminecoin/safeminex)

Website [https://www.safeminecoin.xyz](https://www.safeminecoin.xyz) 

Block Explorer [https://explorer.safeminecoin.xyz](https://explorer.safeminecoin.xyz)

Community [Discord] [https://chat.safeminecoin.xyz](https://discord.gg/97UjGWGbss)

MiningPool [https://miningpoolstats.stream](https://miningpoolstats.stream/safeminex)

Exchange [https://cratex.io](https://cratex.io/index.php?pair=SMX/DOGE)

What is SafeMineX
----------------

SafeMineX is an experimental digital currency that enables instant payments to
anyone, anywhere in the world. SafeMineX uses peer-to-peer technology to operate
with no central authority: managing transactions and issuing money are carried
out collectively by the network. SafeMineX Core is the name of open source
software which enables the use of this currency.

For more information, as well as an immediately useable, binary version of
the SafeMineX Core software, see [https://safeminecoin.xyz](https://safeminecoin.xyz).


## Coin specifications
&nbsp; | &nbsp;
------ | ------
**Coin name** | SafeMineX / SafeMineCoin X
**Coin Ticker** | SMX
**Total number of coins** | 100 000 000 SMX
**Initial block reward** | 100 SMX
**Block halving** | every 500 000 blocks
**Algorithm** | YescryptR16 (PoW / CPU only)
**RPC Port** | 42122
**P2P Port** | 42022
**Public address** | S
**Testnet address** | T
**Average block time** | 1 minute
**Difficulty retarget** | Every block
**Premine** | none


License
-------

SafeMineX Core is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/safeminex-project/safeminex/tags) are created
regularly to indicate new official, stable release versions of SafeMineX Core.

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://groups.google.com/forum/#!forum/safeminex-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer IRC can be found on Freenode at #safeminex-dev.

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

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.
These tests can be run (if the [test dependencies](/qa) are installed) with: `qa/pull-tester/rpc-tests.py`

The Travis CI system makes sure that every pull request is built for Windows, Linux, and OS X, and that unit/sanity tests are run automatically.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.

Translations
------------

We only accept translation fixes that are submitted through [Bitcoin Core's Transifex page](https://www.transifex.com/projects/p/bitcoin/).
Translations are converted to SafeMineX periodically.

Translations are periodically pulled from Transifex and merged into the git repository. See the
[translation process](doc/translation_process.md) for details on how this works.

**Important**: We do not accept translation changes as GitHub pull requests because the next
pull from Transifex would automatically overwrite them again.
