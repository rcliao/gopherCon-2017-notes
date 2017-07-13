# Generate machine code with SSA

Looking at the assembly code to compare performance/efficiency out of Go 1.5
compiler.

Convert from syntax-tree IR to SSA based IR.

Go 1.8 is on SSA based IR. (smaller and faster)

SSA -> Static Single Assignment -> One assignment per variable in the program.

SSA => Control Flow Graph with SSA in it

And a lot of optimizations!
