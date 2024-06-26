_This is the CORW repository for Ari._

Ari
===

Status: _In Progress_

Ari is a
[virtual machine](https://en.wikipedia.org/wiki/Virtual_machine)
to support what might become _Ariadne IV_.

Ari is a virtual machine and a virtual
reduced instruction set computer
\[[RISC](https://en.wikipedia.org/wiki/Reduced_instruction_set_computer)\].

Goals
-----

 1. Simplicity (small code size, including code to compile Ari)
 2. Composability (multiple copies of Ari should be able to work together)

Design Choices
--------------

- Program the computer on the computer.
- Only "printing text" is written to the standard error stream.
- Describable in Standard C with no other dependencies, with a few minor exceptions.
- Single-stepping is facilitated.
- Architecture and instruction set mesh with Forth.
- An 8-bit data stack facilitates the transfer of data between operations.

### Benchmarks

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

Language
--------

Ari is written in C.

Read More
---------

\[[HERE](./var/opt/o0472141737327211107121024131553700252703263/share/doc/index.md)\]
