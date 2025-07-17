# `PaperPC` syntax highlighting

VSCode extension supporting  syntax highlighting for the [`PaperPC`](https://github.com/dluman/paperpc)
assembly/computer organization teaching tool. 

PPC programming relies on a stored-program computer model simiar to the 
[Little Man Computer](https://en.wikipedia.org/wiki/Little_man_computer) and Bell Labs 
[CARDIAC](https://en.wikipedia.org/wiki/CARDboard_Illustrative_Aid_to_Computation). The
`PaperPC` serves to instruct undergraduate computer science students using an assembly-
based approach, featuring an ISA demonstrated by the following basic addition program:
```
1    901    @ Read one value from input to Accumulator
2    320    @ Store in memory location 020
3    901    @ Read one value from input to Accumulator
4    630    @ Unconditional branch to data in 048
30   160    @ Add data in 060 to Accumulator
31   902    @ Output the sum stored in the Accumulator
32   000    @ Halt
```
Each line number represents a value in a memory cell followed by a tab (at least 2 spaces)
with a three-number opcode. Comments follow the approach of most traditional assemblies,
being offset by a `@`.

For a more details about the tool visit the repository linked above.

## Release Notes

### 1.0.0

Initial release of `PaperPC` syntax highlighting.