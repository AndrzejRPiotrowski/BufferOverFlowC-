# BufferOverFlowC-
BufferOverFlow


corrupt memory apart from buffer overflows.
StructLayoutKind.Explicit
Wrong native interop signatures


Buffer Overrun Internal

Buffer overflows is one of the costliest security vulnerabilities known to affect computer software. When input is larger than the space allocated for it, but it is written there anyhow and the memory is overwritten outside the allocated location. In some cases, overflows result from incorrect handling of a mathematical operation or attempts to use memory after the memory has already been allocated. Although many overflows occurs when the program receives more data than it expects, in fact there are many kinds of overflows. It is important to distinguish among various classes of overflows to be able to develop good test cases to identify specific types of overflows.

Integer overflow: Occurs when a specific data type of a CPU register that is meant to hold values within a certain range is to be assigned a value outside that range. Integer overflow often leads to buffer overflow for cases in which integer overflow occurs when computing the size of the memory to allocate.

Stack Overflows: such overflows occur when data is written past the end of buffers allocated on the stack.

Heap Overflow: It occurs when data is written outside the space that was allocated for it on the heap.

Format String Attacks: Format String attacks occur when the %n parameter of the format string is used to write data outside the target buffer.
It is important to delve deep into CPU internal infrastructure by examine various registers that play a significant role during memory allocation.

EIP [Extended Instructor Pointer]: It is only administrated by the CPU and determines the next machine instruction in memory to be executed. They contain the offsets of data and instructions.

ESP [Extended Stack Pointer]: It points to the top of the stack for the CPU to do push and pop operations.

EBP [Extended Base Pointer]: It is used to as reference memory for indirect addressing.

EAX/EBX/ECX/EDX: They are used for arithmetic and data movement.

Segments [CS/DS/SS/FS/ES/GS]: They are used as a base location for program data, instructions and the stack.
