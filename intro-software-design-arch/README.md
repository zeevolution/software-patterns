# Introduction to Software Design Architecture

In here, we are going to study the basics of software design architecture based on the book [`Introdução à Arquitetura de Design de Software`](https://www.amazon.com.br/Introdu%C3%A7%C3%A3o-%C3%A0-Arquitetura-Design-Software/dp/8535250298) by Paulo Silveira.

I chose this book because it is the best reading I had ever had on the subject while I was striving to improve my software development skills as a young software engineer.

The book uses the Java Platform for its software development approach, so we are going to do the same as well.

Next, we are going to follow the same chapters covered by the book:

- [Introduction to Software Design Architecture](#)
- [The Java Platform](#the-java-platform)
- [The Java Virtual Machine](#)
- [Object Oriented Programming Topics](#)
- [Software Responsibilities](#)
- [Tests and Automation](#)
- [Architecture Decisions](#)
- [Web and REST system integrations](#)

## The Java Platform

Understanding your development ecosystem is a must for designing and architecturing good software. Knowing the strengths and weaknesses of the development platforms we want to work with reveals the advantages and limitations we may use and face during our software development projects. Therefore, we are now going to take a brief look into the Java Platform, one of the most used and successful software development and executing technologies in the world.

Standardly released for the first time back in [1996](https://www.codejava.net/java-se/java-se-versions-history), Java has been created for serving as a software development & execution platform. It was built based on three pilars:

- The Java Virtual Machine (JVM)
- Its APIs
- The Java language

The JVM plays as the key role in the Java platform. It enables Java programs to be compiled and executed abstractly for both hardware and operating systems.

> What the heck does that mean?

A [C compiler](https://gcc.gnu.org/) turns a [C programm](https://www.programiz.com/c-programming) into the specific hardware instructions. The generated executable program is made to run only on that specific machine it was compiled on. If you try to run that the executable in another machine or operating system (OS), it will certainly break.

On this such scenario, a C program needs to be compiled for each machine and OS we want it to be executed on:

![C Compiler](images/c_compiler.png)

On the other hand, the JVM makes those portability cases a lot simpler. A Java compiler generates an executable program for a **generic application virtual machine**, the JVM. The JVM is a specification of a complete virtual machine which is responsible for abstracting the communication with the Operating System and its hardware. Therefore, instead of compiling a Java program for each running machine/OS, we can simply provide them a JVM environment, so they all can run the same executable program through that virtual machine.

> You may feel free to argue that we still depend on a JVM environment specifically for each machine or operating system we want to work with. That is a fact!! However, once we have these JVM implementations, we can execute any Java program which is compatible with that JVM implementation.

In order to enable such scenarios, the Java platform offers the follwing two software pieces:

- **The JDK (Java Development Kit):** contains the JVM machine, APIs and Java Language for enabling software development.

- **The JRE (Java Runtime Environment):** contains the JVM machine and APIs for executing Java compiled programs.

![Java Compiler](images/java_compiler.png)
