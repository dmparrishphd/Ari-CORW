Character Sets
==============

The Basic-Graph,<br>
Basic-Print, and<br>
Basic-Text<br>
Character Sets
--------------------

The _basic-graph_ characters are those of the Unicode subrange
`U+0021` to `U+007e`, except `U+0024` (DOLLAR SIGN), `U+0040` (AT SIGN), and `U+0060` (GRAVE ACCENT):

    ABCDEFGHIJKLMNOPQRSTUVWXYZ
    abcdefghijklmnopqrstuvwxyz
    0123456789
    !"#%&'()*+,-./:;<=>?[\]^_{|}~

The _basic-print_ characters include the _basic-graph_
characters and the _space_ (`U+0020`) character only.

The _basic-text_ characters include the _basic-print_ and _newline_
characters only.

The A-Graph,<br>
A-Print, and<br>
A-Text<br>
Character Sets
----------------

The _a-graph_ characters include the _basic-graph_ characters as well as `U+0024` (DOLLAR SIGN), `U+0040` (AT SIGN), and `U+0060` (GRAVE ACCENT); i.e., `U+0021` to `U+007e`, inclusive.

The _a-print_ characters include the _a-graph_ and space (`U+0020`) characters only.

The Execution Character Set
---------------------------

A requirement of the system simulating Ari is that the execution character set include in a continuous range of positively-valued `char`-s the _a-graph_ characters. This allows determination of whether a character is an _a-graph_ character in O(0) time complexity.

________________________________________________________________

[INDEX](../../index.md)
