Introduction
============

Pixie is a lightweight lisp suitable for both general use as well as shell scripting. The standard library is heavily inspired by Clojure as well as several other functional programming languages. It is written in RPython and as such supports a fairly fast GC and an amazingly fast tracing JIT.

Pixie implements its own virtual machine. It does not run on the JVM, CLR or Python VM. It implements its own bytecode, has its own GC and JIT. And it's small. Currently the interpreter, JIT, GC, and stdlib clock in at about 10.3MB once compiled down to an executable

If you like Clojure, but are unhappy with the start-up time, or if you want something outside of the JVM ecosystem, then Pixie may be for you. 

**Pixie is still in a "pre-alpha" phase and as such changes fairly quickly.**

**This documentation is also still in development**