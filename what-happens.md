# What happens when I create a program?
In this chapter we're going to analyze what happens between writing and running a program. We'll look at 4 different languages, you don't have to know all 4, but you should have heard of them. 

## C++
C++ is a *compiled language*. C++ is run through a compiler and becomes an executable. The source language is C++, and the target language is an executable. The compiler does not go straight from C++ to an executable though, that is difficult to do and annoying to implement. It first converts C++ into *assembly*, passes the assembly into an *assembler*, and that assembler gives us an executable. 

#### Assemblers and assembly
What in the world is assembly? You may have heard of it before and you may be scared of it, but you shouldn't be. Our computers are dumb, they don't know what strings are, they don't know how to loop, they just have some simple commands. They can also only understand binary. `1001 0011 0100` might tell the computer to perform the computation `3 + 4`. That's not human readable! This is where assembly comes in. Instead of writing `1001` when you want to add two numbers, you just write `add 3 4`. That's much better! The job of the assembler is to convert this human readable assembly into a machine readable executable. 

## Java
There are two steps to run a Java program. First, you must compile it like C++, then you must pass it into the VM. When you run the command `javac`, the Java compiler converts your code from Java, to Java bytecode. Once your program is in bytecode, it can be ran by the `java` command. The command launches the Java Virtual Machine, JVM for short, and it processes the bytecode. The source language is Java, and the target language is JVM bytecode.  

#### Bytecode and Virtual Machines
A Virtual Machine simulates the simplicity of our computer. Most VMs have simple commands, such as those for adding or subtracting, but they might have built in support for more complicated things like strings or loops. These VMs take input in bytecode. Bytecode is similar to an executable. However, unlike an executable, bytecode is not run by the computer, bytecode is run by the VM.

## Typescript
Typescript is a *transpiled language*. Transpilers are similar to a tool one might use to convert .png images into .jpg images, but instead of images they work with languages. In the case of Typescript, it outputs Javascript. We can say that the source language is Typescript, and the target language is Javascript. Now you can run your code just like any other Javascript code you'd like to run. Some may argue that a compiler is really just a specfic case of a transpiler. 

## Ruby
Ruby is an *interpreted language*. What makes an interpreted language special is that they do not have any target language. The program is run through an interpreter, which gives you a result without any other steps. There is no intermediate step of compilation. If you ask Ruby to run the code `3 + 4`, it will do it instantly. One of the tradeoffs of using an interpreted language is that they are generally slower, the interpreter must do all of the work when the program is run. However, interpreted languages are portable and much simpler to run than compiled languages. We will discuss the speed tradeoffs in later sections of the book. 
