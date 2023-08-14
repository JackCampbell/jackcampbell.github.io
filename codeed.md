<link rel="stylesheet" type="text/css" href="https://fonts.googleapis.com/css?family=Ubuntu:regular,bold&subset=Latin">
<style>
	* {
		font-family: Ubuntu, "times new roman", times, roman, serif;
	}
	img { max-width: 400px; }
</style>

# CodeEd

![CodeEd](assets/codeed-s.png)

It is an IDE designed for developing applications and units in C/C++ environments. It is being developed from 2020, taking as an example of low power consumption and simple use.

> B.Firat.OZDEMIR  
> Software Engineer


> I am actively using it in many projects.

## C/C++ Tools

The CodeEd application provides a number of features in the C/C++ environment.

#### Auto Complete

Detailed Description Code completion involves taking an (incomplete) source file, along with knowledge of where the user is actively editing that file, and suggesting syntactically- and semantically-valid constructs that the user might want to use at that particular point in the source code.

#### Code Tip

It ensures that the functions in the source files in the project are called correctly and the default arguments are displayed.

#### Diagnostics

It notifies the software developer of errors or warnings that may be made during operation. It can be displayed as a list with the diagnosis panel. This feature can be changed in the application settings.

| ![1](assets/codeed-2.png) | ![1](assets/codeed-1.png) | ![1](assets/codeed-3.png) |
|-|-|-|

#### Compile Command

A build database holds all the information used to compile files in a project. For each file in the database, the working directory or the command line used for the compiler call can be queried. It allows transforming the source files in the project. It ensures that the equipment works correctly on the project.

#### Serialize

By serializing the system files associated with your projects, it enables the source files to be translated more quickly. You need to add the Precompiled header file in your project and activate the application settings. It re-serializes the precompiled header file every time it is changed.

#### Indexer

The project navigates the source files found and stores the found classes and functions in a database environment. this storage data is used by spotlight dialog and new function declaration. The source code you are working on is check again during document save. This check again during document save provide at new function declare. It can be changed in the application settings dialog.

#### Spotlight

It creates a database by collecting all the collections on the project. Allows you to search for functions, classes, and files while running.

| ![1](assets/codeed-e.png) | ![1](assets/codeed-d.png) |
|-|-|

#### Code-Format

Code-formatter is a tool that automatically formats C/C++ code so developers don't have to worry about style issues during code reviews. It is highly recommended that you format your modified C++ code before opening pull requests, this will save you and your reviewers time. The CodeEd implementation uses the clang-formatter API. There are certain formats in the settings dialog or a custom format can be created by reading the '.clang-format' file within the project.

#### Debug

In general, a debugger is a computer program that helps test and debug other programs. LLDB and GDB are two debuggers. CodeEd includes LLDB API.

![1](assets/codeed-5.png)

It offers some of the capabilities that this debugger will give you over trace messages in the code:
* It displays the call stack at any time, giving you a context for your current stack frame.
* Change variable values while the program is running
* Edit and continue - ability to modify code as it works and see the results of the change immediately
* Being able to monitor variables, see when they change
* You can skip or repeat code sections to see how the code will perform. This allows you to test theoretical changes before making them.
* Inspect memory content in real time
* Alerts you when certain exceptions are thrown, even if they are being handled by the application.
* Conditional interrupt; stopping the application only in exceptional cases to allow you to analyze the stack and variables.
* Display thread context in multi-threaded applications, which can be difficult to achieve with tracing (because traces from different threads will be interspersed in the output).
* In summary, print statements are (usually) static, and if your original statements are not verbose enough, you'll need to recompile them to get additional information. The IDE removes this static barrier, giving you a dynamic toolset at your fingertips.
* When I first started coding I didn't realize how important debuggers were and thought I could accomplish anything with tracing (agreed, this was on unix and the debugger was GDB). But once you learn how to properly use a graphical debugger, you don't want to go back to printing expressions.

| Breakpoints | Call Stack | Watch |
|-|-|-|
| ![1](assets/codeed-6.png) | ![1](assets/codeed-7.png) | ![1](assets/codeed-8.png) |

## Process

It allows you to test the project you are working on after it is compiled. This test process is provided by the user specifying the configuration. With the configuration arguments and macro the specified target remains the same even when the file is moved.

| Process Panel | Config Dialog | Macro Panel |
|-|-|-|
| ![1](assets/codeed-a.png) | ![1](assets/codeed-b.png) | ![1](assets/codeed-c.png) |

## Builder Form

application development and user-friendly form desktop design support. It uses the wxWidgets environment.

| Resource Edit | Design Edit |
|-|-|
| ![1](assets/codeed-9.png) | ![1](assets/codeed-f.png) |

# Javascript and Python Support

Ancillary equipment for developing code in Javascript and Python projects.

| Javascript | Python |
|-|-|
| ![1](assets/codeed-g.png) | ![1](assets/codeed-i.png) |
| ![1](assets/codeed-h.png) | ![1](assets/codeed-j.png) |


# CMake Support

It allows you to compile in a multi-platform environment with CMake support.

![1](assets/codeed-k.png)

# Document

Markdown format support for documentation in your project.

![1](assets/codeed-l.png)


## Other Support

* Image Editor
* Image Processing
* Medical Monitor
* Scientist
* Database
* Hex Editor
* GLSL shader support.
* Language Server Protocol (LSP) support. (experimental)


| ![1](assets/codeed-m.png) | ![1](assets/codeed-n.png) | ![1](assets/codeed-o.png) |
|-|-|-|
| ![1](assets/codeed-p.png) | ![1](assets/codeed-q.png) | ![1](assets/codeed-r.png) |


---
> © 2021. B. Firat OZDEMIR. All rights reserved.
