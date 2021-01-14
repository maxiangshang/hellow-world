# Mode, privilege and stack pointer are key concepts used in ARMv7-M.
## Mode
An M-profile processor supports two operating modes:  
**Thread mode** Is entered on reset, and can be entered as a result of an exception return.  
**Handler mode** Is entered as a result of an exception. The processor must be in Handler
mode to issue an exception return.
## Privilege
Code can execute as privileged or unprivileged. Unprivileged execution limits or excludes access to
some resources. Privileged execution has access to all resources.
Execution in Handler mode is always privileged. Execution in Thread mode can be privileged or unprivileged.
Stack pointer The processor implements a banked pair of stack pointers, the Main stack pointer, and the Process
stack pointer. See *The SP registers on page B1-516* for more information.
In Handler mode, the processor uses the Main stack pointer. In Thread mode it can use either stack
pointer.

