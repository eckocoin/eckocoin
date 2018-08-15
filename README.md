ECKO [ECKO] integration/staging tree
=====================================

http://www.eckocoin.com

What is the ECKO [ECKO] Blockchain?
---------------------------

The ECKO [ECKO] Blockchain is an experimental smart contract platform protocol that enables 
instant payments to anyone, anywhere in the world in a private, secure manner. 
ECKO [ECKO] uses peer-to-peer blockchain technology developed by Bitcoin to operate
with no central authority: managing transactions, execution of contracts, and 
issuing money are carried out collectively by the network. ECKO [ECKO] is the name of 
open source software which enables the use of this protocol.

Coin Specs
----------

<table>
<tr><td>Coin name</td><td>ECKOCoin</td></tr>
<tr><td>Coin ticker</td><td>ECKO</td></tr>
<tr><td>Algorithm</td><td>X13</td></tr>
<tr><td>Block time</td><td>60 sec</td></tr>
<tr><td>Port</td><td>15391</td></tr>
<tr><td>RPC Port</td><td>15392</td></tr>
<tr><td>Address Prefix</td><td>E</td></tr>
<tr><td>Type</td><td>POS/MN</td></tr>
<tr><td>Max Total Supply</td><td>400 000 000 ECKO</td></tr>
<tr><td>Premine</td><td>300 000 000 ECKO</td></tr>
<tr><td>POS Rate</td><td>10% per Annum</td></tr>
<tr><td>Coin Age</td><td>24 hours</td></tr>
<tr><td>Masternode Collateral</td><td>1 00 000 ECKO</td></tr>
<tr><td>Confirmation</td><td>15 blcok</td></tr>
<tr><td>Masternode Rate</td><td>30% of POS</td></tr>
</table>

BUILD LINUX
-----------

1) git clone https://github.com/eckocoin/eckocoin

2) cd eckocoin/src

3) sudo make -f makefile.unix            # Headless

(optional)

4) strip ECKOd

5) sudo cp ECKOd /usr/local/bin

License
-------

ECKO [ECKO] is released under the terms of the MIT license. See [COPYING](COPYING) for more
information or see https://opensource.org/licenses/MIT.

Development Process
-------------------

The `master` branch is regularly built and tested, but is not guaranteed to be
completely stable. [Tags](https://github.com/CryptoCoderz/ECKO/tags) are created
regularly to indicate new official, stable release versions of ECKO [ECKO].

The contribution workflow is described in [CONTRIBUTING.md](CONTRIBUTING.md).

The developer [mailing list](https://lists.linuxfoundation.org/mailman/listinfo/bitcoin-dev)
should be used to discuss complicated or controversial changes before working
on a patch set.

Developer Slack can be found at http://eckocointeam.slack.com.

Testing
-------

Testing and code review is the bottleneck for development; we get more pull
requests than we can review and test on short notice. Please be patient and help out by testing
other people's pull requests, and remember this is a security-critical project where any mistake might cost people
lots of money.

### Automated Testing

Developers are strongly encouraged to write [unit tests](/doc/unit-tests.md) for new code, and to
submit new unit tests for old code. Unit tests can be compiled and run
(assuming they weren't disabled in configure) with: `make check`

There are also [regression and integration tests](/qa) of the RPC interface, written
in Python, that are run automatically on the build server.

### Manual Quality Assurance (QA) Testing

Changes should be tested by somebody other than the developer who wrote the
code. This is especially important for large or high-risk changes. It is useful
to add a test plan to the pull request description if testing the changes is
not straightforward.
