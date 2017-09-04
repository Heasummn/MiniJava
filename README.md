# MiniJava

## What is this book about?
This book is supposed to teach people about the theory and work that goes into making a compiler. We will work through the different parts of a compiler, and then look at the implementation for a small language. Hopefully it will leave you, the reader, with enough knowledge to implement a compiler of your own. 

## Hold up, what in the world is a compiler?
If you're reading this book, you've probably used a compiler in the past, but that doesn't necessarily mean you know what it is, or how it works. A compiler has a simple job, it transforms code written in some language to code written in some other language. But we can be even more abstract, all a compiler really does is take some input, and changes it to something else. 

You've probably used a calculator before, you give the calculator some input `3 + 4`, and it will give you some output, like `7`. That is in essence, all a compiler does. 

A compiler takes in a "source language", and outputs a "target language". In the case of our calculator the source language is a mathematical expression, and the target language is also a mathematical expression. If you've used Java, the source language is Java, and the target language is JVM bytecode (if you've never heard that word before, don't worry, we will discuss it in later sections of this book). 

## What is "MiniJava"?
MiniJava is a subset of the Java programming language. It was created by Andrew Appel as a source language for his compiler books, we will modify it a bit and use it as the source language for this book. You do not need to know Java to understand MiniJava, however some knowledge of OOP is helpful. We won't be discussing MiniJava for quite some time, so don't worry about it for now. 
