# Screenshots

Enter the binary and args just as you'd call them on the command line.
Binary is restored when gdbgui is opened at a later time.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/load_binary_and_args.png)

Intuitive control of your program. From left to right: Run, Continue,
Next, Step, Return, Next Instruction, Step Instruction.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/controls.png)

## Stack/Threads

View all threads, the full stack on the active thread, the current frame
on inactive threads. Switch between frames on the stack, or threads by
pointing and clicking.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/stack_and_threads.png)

## Send Signal to Inferior
Choose from any signal your OS supports to send to the inferior. For example, to mock `CTRL+C` in plain gdb, you can send `SIGINT` to interrupt the inferior process. If the inferior process is hung for some reason, you can send `SIGKILL`, etc.
![image](https://github.com/cs01/gdbgui/raw/master/screenshots/send_signal.png)

Signals are also recognized by `gdbgui`, and a button is presented to let you step back into the program and inspect the program's state in case it exits unexpectedly.
![image](https://github.com/cs01/gdbgui/raw/master/screenshots/SIGSEV.png)


## Source Code
View source, assembly, add breakpoints. All symbols used to compile the
target are listed in a dropdown above the source code viewer, and have
autocompletion capabilities. There are two different color schemes: dark (monokai), and a light theme (default).

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/source.png)

With assembly. Note the bold line is the current instruction that gdb is
stopped on.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/source_with_assembly.png)

If the source file is not found, it will display assembly, and allow you to step through it as desired.
![image](https://github.com/cs01/gdbgui/raw/master/screenshots/assembly.png)


## Variables and Expressions

All local variables are automatically displayed, and are clickable to
explore their fields.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/locals.png)

Hover over a variable and explore it, just like in the Chrome debugger.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/hover.png)

Arbitrary expressions can be evaluated as well. These expressions persist as the program is stepped through. The base/radix can be modified as desired.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/expressions.png)

Expressions record their previous values, and can be displayed in an x/y
plot.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/plots.png)

Expressions can be interactively explored in a tree view.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/tree_explorer.png)


## Memory Viewer

All hex addresses are automatically converted to clickable links to
explore memory. Length of memory is configurable. In this case 10 bytes
are displayed per row.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/memory.png)

## Registers

View all registers. If a register was updated it is highlighted in
yellow.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/registers.png)

## gdb console

Read gdb output, and write to the gdb subprocess as desired. Don't let
any gdb commandline skills you've developed go to waste.

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/console.png)

## gdbgui at launch

![image](https://github.com/cs01/gdbgui/raw/master/screenshots/ready.png)


