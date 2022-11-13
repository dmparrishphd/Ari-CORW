Processing
==========

Words in the _Queue_ are processed in the order encountered.

The _Lexicon_ is searched for the next word in the _Queue_.

If the word is not found in the _Lexicon_, it is added to the _Lexicon_.

The _Dictionary_ is searched for the word.

If the word is not found in the _Dictionary_, the word is placed on the _Word Stack_.
Otherwise, the code associated with the word is executed.
