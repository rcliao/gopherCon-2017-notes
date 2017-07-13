# A Go Programmer's Guide to Syscalls

Use *syscalls* to set up containers.

## What are syscalls?

> It's a way requesting services from the kernel of the operating system.

It's a portability layer. In other word, implementing syscalls interface =>
emulate linux.

## How syscalls work

Set up register and send it to kernel to execute. Expect a return value (reference)
by the end of method.

## Fun with ptrace

60 lines of code to implement strace.

> Live demo

https://github.com/lizrice/strace-from-scratch

## Syacalls and security

* Seccomp restricts permitted syscalls
