# What happens when I create a program?
In this chapter we're going to analyze what happens in between writing and running a program. We'll look at 4 different languages, you don't have to know all 4, but you should have at least heard of them. 

## C++
C++ is a *compiled language*. This means that C++ code is run through a compiler and that compiler returns an executable, something that your operating system can understand. This is what we will be implementing in this book, a language that can be ran on your computer. We can say that in this case, the source language is C++, and the target language is an executable. The compiler does not go straight from C++ to an executable though, that is difficult to do and annoying to implement. It first converts the C++ into something known as *assembly* and then converts the assembly into an executable. 

#### Assembly
What in the world is assembly? You may have heard of it before, and you may be scared of it, but you shouldn't be, assembly is really simple. Our computers are dumb, they don't know what strings are, they don't know how to loop, they just have some simple commands. The Computers can only do things like add numbers. To tell a computer to add two numbers, such as 3 and 4, you have to tell it in binary. You have to ive it something like `1001 0011 0100`. That's not human readable! This is where assembly comes in. Instead of writing `1001` when you want to add two numbers, you just write `add`. Instead of writing the number out in binary, you write it in decimal. The compiler then converts your commands and numbers into their binary equivalent.  

I talked about how the computer is stupid, and it cannot do complicated tasks, such as loops on its own. How then, do we get things like loops in our programming languages? That's the job of the compiler! The compiler takes our complicated, messy code, and turns it into basic tasks that the computer can do. 

## Java
Java is a bit more complicated than our previous two. To run a Java program, you need to take two steps, first you must compile it, and then you must pass it into the VM. Java is, like C++, a *compiled language*, however it is also run through a virtual machine. When you run the command `javac`, a program is run, this program takes your Java code, and converts it into something known as *bytecode*. Once your program is in bytecode, it can be ran by the `java` command. The command launches the Java Virtual Machine, JVM for short, and it processes the bytecode. The source language is Java, and the target language is JVM bytecode.  

#### Bytecode and Virtual Machines
Virtual Machines are exactly what they're named, virtual representations of a machine. A VM simulates our stupid computers, but also while being a bit smarter. Most VMs have simple commands, such as those for adding or subtracting, but they might have built in support for things like strings or loop. These VMs take input in bytecode. Bytecode is similar to an executable. It has commands for adding numbers and the like written in binary. However, unlike an executable, bytecode is not ran by the computer, bytecode is ran by a VM.

## Typescript
Typescript is a *transpiled language*. This means that it's code is run through a transpiler, and that transpiler can output any language. Transpilers are kind of like converters, such as a tool to convert .png images into .jpg images, but instead of images they work with languages. In the case of Typescript, it outputs another language, known as Javascript. We can say that the source language is Typescript, and the target language is Javascript. Now you can run your code just like any other Javascript code you'd like to run. Some may argue that a compiler is really just a specfic case of a transpiler. 

## Ruby
Ruby is an *interpreted language*. What makes an interpreted language special is that they do not have any target language. The program is run through an interpreter, which gives you a result without any other steps. Running a ruby program, your code goes straight from source code to being run. There is no intermediate step of compilation. If you ask ruby to run the code `3 + 4`, it will do it instantly. One of the tradeoffs of using an interpreted language is that they are generally slower, the interpreter must do all of the work when the program is run. We will look more into the speed tradeoffs later, as we discuss the internals of a compiler.

