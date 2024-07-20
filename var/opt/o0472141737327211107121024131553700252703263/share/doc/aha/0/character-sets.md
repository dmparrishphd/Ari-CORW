Character Sets
==============

Basic-Graph, Basic-Print, and Basic-Character Character Sets
------------------------------------------------------------

The _basic-graph_ characters are those of the Unicode subrange
U+0021 to U+007e, except U+0024, U+0040, and U+0060:

    ABCDEFGHIJKLMNOPQRSTUVWXYZ
    abcdefghijklmnopqrstuvwxyz
    0123456789
    !"#%&'()*+,-./:;<=>?[\]^_{|}~

The _basic-print_ characters include the _basic-graph_
characters and the _space_ character only.

The _basic-characters_ include the _basic-print_ and _newline_
characters only. The _basic-characters_ are also called the _basic-text_ characters.

The A-Graph, A-Print, and A-Text Character Sets
--------------------------------------------------

The _a-graph_ characters include the _basic-graph_ characters as well as U+0024, U+0040, and U+0060, i.e., U+0021 to U+007e, inclusive.

The _a-print_ characters include the _a-graph_ and space (U+0020) characters only.

A requirement of the system simulating Ari is that the execution character set include in a continuous range of positively-valued `char`-s the _aprint_ characters.

________________________________________________________________

[INDEX](../../index.md)
