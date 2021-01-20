# virtual-machine

So why build a virtual machine? Firstly, I find machine emulation to be an interesting problem to solve, and secondly I also 
want a better understanding of how a computer works. Most software engineers, including myself, work within layers of 
abstraction without a real understanding of how the magic sauce is made. So this is my stab at writing a full MIPS based 
Virtual Machine in Java. 

#### Table of Contents

- [What is a Virtual Machine?](#vmDescription)

<a name="vmDescription">What is a virtual Machine?</a>
---
So what is a virtual machine? Well, in its simplest form, a virtual machine is creating a computer within a computer. It's a 
piece of software that runs on a physical machine that emulates another machine. 

Take Java for instance, Java runs on a virtual machine. When you write a program and compile it, you're effectively 
producing Java bytecodes. The bytecode is a sequence of instructions for a non-existent CPU which the JVM emulates. When
you load a class file, your jvm simply sequences through the instructions in your java program, emulating each bytecode 
one at a time. While a JVM can have some more complex behaviors, at it's core, a virtual machine is simply a piece of 
software that emulates a foreign instruction set.

My virtual machine is going to act like a JVM, but emulating MIPS instructions instead of Java bytecodes.


 






