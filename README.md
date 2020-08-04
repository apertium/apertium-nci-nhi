nhi and nhn: `apertium-nhi-nhn`
===============================================================================

This is an Apertium language pair for translating between nhi and
nhn. What you can use this language package for:

* Translating between nhi and nhn
* Morphological analysis of nhi and nhn
* Part-of-speech tagging of nhi and nhn

For information on the latter two points, see subheading "For more
information" below.

Requirements
-------------------------------------------------------------------------------

You will need the following software installed:

* lttoolbox (>= 3.5.1)
* apertium (>= 3.6.1)
* vislcg3 (>= 1.3.1)
* hfst (>= 3.15.1)
* apertium-nhi
* apertium-nhn

If this does not make any sense, we recommend you look at: www.apertium.org.

Compiling
-------------------------------------------------------------------------------

Given the requirements being installed, you should be able to just run:

```console
$ ./configure
$ make
# make install
```

You can use `./autogen.sh` instead of `./configure` in case you're compiling
from source. If you installed any prerequisite language packages using a
`--prefix` with `./configure`, make sure to use the same `--prefix` when running
`./configure` here.

Testing
-------------------------------------------------------------------------------

If you are in the source directory after running make, the following
commands should work:

```console
$ echo "TODO test sentence 1" | apertium -d . nhi-nhn
TODO test translated sentence 1

$ echo "TODO test sentence 2" | apertium -d . nhn-nhi
TODO test translated sentence 2
```

After installing somewhere in `$PATH`, you should be able to do e.g.

```console
$ echo "TODO test sentence 1" | apertium nhi-nhn
TODO test translated sentence 1
```

Files and data
-------------------------------------------------------------------------------

* [`apertium-nhi-nhn.nhi-nhn.dix`](apertium-nhi-nhn.nhi-nhn.dix) - Bilingual dictionary
* [`apertium-nhi-nhn.nhi-nhn.t1x`](apertium-nhi-nhn.nhi-nhn.t1x) - Chunking rules for translating into nhn
* [`apertium-nhi-nhn.nhn-nhi.t1x`](apertium-nhi-nhn.nhn-nhi.t1x) - Chunking rules for translating into nhi
* [`apertium-nhi-nhn.nhi-nhn.t2x`](apertium-nhi-nhn.nhi-nhn.t2x) - Interchunk rules for translating into nhn
* [`apertium-nhi-nhn.nhn-nhi.t2x`](apertium-nhi-nhn.nhn-nhi.t2x) - Interchunk rules for translating into nhi
* [`apertium-nhi-nhn.nhi-nhn.t3x`](apertium-nhi-nhn.nhi-nhn.t3x) - Postchunk rules for translating into nhn
* [`apertium-nhi-nhn.nhn-nhi.t3x`](apertium-nhi-nhn.nhn-nhi.t3x) - Postchunk rules for translating into nhi
* [`apertium-nhi-nhn.nhi-nhn.lrx`](apertium-nhi-nhn.nhi-nhn.lrx) - Lexical selection rules for translating into nhn
* [`apertium-nhi-nhn.nhn-nhi.lrx`](apertium-nhi-nhn.nhn-nhi.lrx) - Lexical selection rules for translating into nhi
* [`apertium-nhi-nhn.nhi-nhn.lsx`](apertium-nhi-nhn.nhi-nhn.lsx) - Discontiguous multiword rules for translating into nhn
* [`apertium-nhi-nhn.nhn-nhi.lsx`](apertium-nhi-nhn.nhn-nhi.lsx) - Discontiguous multiword rules for translating into nhi
* [`modes.xml`](modes.xml) - Translation modes

For more information
-------------------------------------------------------------------------------

* http://wiki.apertium.org/wiki/Installation
* http://wiki.apertium.org/wiki/apertium-nhi-nhn
* http://wiki.apertium.org/wiki/Using_an_lttoolbox_dictionary

Help and support
-------------------------------------------------------------------------------

If you need help using this language pair or data, you can contact:

* Mailing list: apertium-stuff@lists.sourceforge.net
* IRC: `#apertium` on irc.freenode.net (irc://irc.freenode.net/#apertium)

See also the file [`AUTHORS`](AUTHORS), included in this distribution.
