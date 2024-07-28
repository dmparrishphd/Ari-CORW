Ari
===

Introduction
------------

This is the CORW (create once; read and write many times) repository for Ari.

Ari is a [virtual](https://en.wikipedia.org/wiki/Virtual_machine) [stack machine](https://en.m.wikipedia.org/wiki/Stack_machine) and virtual [reduced instruction set computer (RISC)](https://en.wikipedia.org/wiki/Reduced_instruction_set_computer).

Ari is intended to support Ariadne IV, a dialect of Forth \[[1](http://forth.org), [2](https://forth-standard.org/)\]. Predecessors of Ariadne IV include Ariadne III, one of a few [Python 4th's (Python Forths)](https://github.com/dmparrishphd/Python4th)


Goals
-----

 - Composability: multiple copies of Ari should be able to work together.
 - Comprehensibility: Source code should speak for itself; comments should be unnecessary.
 - Programability: The user should be able to program the computer on the computer without "dev kits," cross compilers, etc.
 - Simplicity: small code size, including code to compile Ari.

Design Choices
--------------

- Only "printing text" is written to the standard error stream.
- Describable in Standard C with no other dependencies, with a few minor exceptions.
- Single-stepping is facilitated.
- Architecture and instruction set mesh with Forth.
- An 8-bit data stack facilitates the transfer of data between operations.

### Benchmarks

 - The [F18A Computer and the GA 144](https://www.greenarraychips.com/home/documents/index.php) a 144-processor supercomputer designed by Chuck Moore and [GreenArrays](https://www.greenarraychips.com/index.html). The F18A has (only) 32 instructions. 
 - The 6502 \[[1](https://westerndesigncenter.com/wdc/documentation/w65c02s.pdf),
 [2](https://en.wikipedia.org/wiki/MOS_Technology_6502),
 [3](http://6502.org/)\]
 is too complicated.
 - RISC-V \[[1](https://riscv.org/),
 [2](https://en.wikipedia.org/wiki/RISC-V)\]
 is too complicated.

Inspiration
-----------

In the film [_The Queens Gambit_](https://www.netflix.com/title/80234304),
the protagonist's (adopted) mother makes a comment about chess,
as she watches her daughter play a match:
"It's so complicated."
Therefore, I am striving to make Ari _less_ complicated than chess
\[[1](https://handbook.fide.com/chapter/E012018),
[2](https://en.wikipedia.org/wiki/Rules_of_chess)\].

Koopman PJ (1989) [Stack Computers: The New Wave](https://users.ece.cmu.edu/~koopman/stack_computers/index.html)

Charles H. "Chuck" Moore.

Ting CH (2013) _eForth and Zen_. Offete Enterprises. [Offete Store](
https://www.forth.org/OffeteStore/OffeteStore.html)

Language
--------

Ari is written in C.

CH Ting and others have several publications in which Forth is fully specified in terms of a machine-specific assembly language. In writing Ari in C, we trade a degree of specificity for a degree of comprehensibility.

Read More
---------

\[[HERE](./var/opt/o0472141737327211107121024131553700252703263/share/doc/index.md)\]
