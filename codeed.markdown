<link rel="stylesheet" type="text/css" href="https://fonts.googleapis.com/css?family=Ubuntu:regular,bold&subset=Latin">
<style>
	* {
		font-family: Ubuntu, "times new roman", times, roman, serif;
	}
	img[alt='icon'] { width: 64px; height: 64px; }
	img[alt='app'] { min-height: 300px; }
	img[alt='giphy'] {
		max-height: 210px;
		display: inline-block;
		margin-right: 16px;
		border: 1px solid #c4c4c4;
	}
	img[alt='dialog'] {
		max-height: 200px;
	}
	img[alt='frame'] {
		max-height: 360px;
	}
	img[alt='frame2'] {
		max-height: 300px;
	}
</style>


# CodeEd

![icon](assets/codeed.png)

CodeEd is based on powerful code editor and developer tools. It was originally designed for application and unit development. It has been developed according to the needs since 2020 based on low power consumption and simple use. _It is actively used in many projects_.

![app](assets/code-main2.png)


## C/C++ Tools

This IDE application provides a number of features in the C/C++ environment.

### Auto Complete

Code completion involves taking an (incomplete) source file, along with knowledge of where the user is actively editing that file, and suggesting syntactically and semantically-valid constructs that the user might want to use at that particular point in the source code.


![giphy](assets/code-autocomplete1.gif)
![giphy](assets/code-autocomplete2.gif)


### Code Tip

It ensures that the functions in the source files in the project are called correctly and the default arguments are displayed. After an unclosed parenthesis for a function, open a small window with function parameter hints.

![giphy](assets/code-calltip1.gif)

### Diagnostics

It notifies the software developer of errors or warnings that may be made during operation. It can be displayed as a list with the diagnosis panel. This feature can be changed in the application settings.

![giphy](assets/code-diagnostic1.gif)

### Build Command Database

A build database contains the arguments used to compile files in a project. For each file in the database, the working directory or the command line used for the compiler call can be queried. It ensures that the source files in the project are properly translated into C/C++ language and that the equipment works correctly on the project.

### Serialization

It serializes the system files associated with your projects, allowing faster translation of source files. You need to add the Precompiled header file to your project and activate the application settings. Each time the Precompiled header file is modified, it re-serializes the system files.

### Indexer [Experimental]

It navigates through the source files in the project and stores the classes and functions found in a database environment. this storage data is used by the spotlight dialog and the new function declaration. The source code you are working on is checked again during document saving. This rechecking during document saving is provided in the new function declaration. Application settings can be changed in the dialog.

### Spotlight

Creates a database by collecting all collections on the project. It allows you to search for functions, classes and files as you work.

![dialog](assets/code-spotlight.png)

### Code-Format

Code-formatter is a tool that automatically formats C/C++ code so that developers don't have to worry about style issues during code reviews. Formatting your C/C++ code is highly recommended, it will save you and your reviewers time. The CodeEd application uses the clang-formatter API. Specific formats are available in the settings dialog, or a custom format can be created by reading the `.clang-format` file within the project.

![giphy](assets/code-format.gif)

### Debug

In general, a debugger is a computer program that helps test and debug other programs. LLDB and GDB are two debuggers. CodeEd includes LLDB API.

![giphy](assets/code-debug.gif)


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
* In summary, print statements are (usually) static, and if your original statements are not verbose enough, you’ll need to recompile them to get additional information. The IDE removes this static barrier, giving you a dynamic toolset at your fingertips.
* When I first started coding I didn’t realize how important debuggers were and thought I could accomplish anything with tracing (agreed, this was on unix and the debugger was GDB). But once you learn how to properly use a graphical debugger, you don’t want to go back to printing expressions.
* lldb-server provides the server counterpart of the LLVM debugger. The server runs and monitors the debugged program, while the user interfaces with it via a client, either running locally or connecting remotely.

![dialog](assets/code-debug2.png)
![dialog](assets/code-watch.png)
![dialog](assets/code-breakpoints.png)

## Process

It allows you to test the project you are working on after it has been compiled. This test is prompted by the user specifying the configuration. The configuration arguments and the target file specified by the macro remain the same even when the file is moved.

![giphy](assets/code-process.gif)


## Design And Resource

It supports application development and user-friendly form desktop design with the wxWidgets environment. This IDE was developed using this equipment.

![frame](assets/code-resource.png)
![frame](assets/code-design.png)

## CMake Support

CMake support allows you to build, automate, test, package and install software in a multi-platform environment.

![frame](assets/code-cmake.png)

## Javascript

Provides support for nodejs projects with a JavaScript runtime environment. Provides autocompletion and function signature at coding time.

![giphy](assets/code-node-autocompletion.gif)
![giphy](assets/code-node-calltip.gif)

## Python

Provides support for projects with Python3 runtime environment. Provides autocompletion and function signature at coding time.

![giphy](assets/code-python-autocompletion.gif)
![giphy](assets/code-python-calltip.gif)

## Documents

![giphy](assets/code-markdown.gif)

* `Markdown` format support for documentation in your project.
* Support for `Sqlite3` format for database analysis in your project.
* Supports `GLSL` to provide more direct control over the graphics pipeline in projects that use graphics processing.
* `Hex Edit` support for allowing manipulation of the underlying binary data that make up a computer file.
* Language Server Protocol (LSP) support. (experimental)


![frame2](assets/code-sqlite3.png) ![frame2](assets/code-hex.png)

## Plans / TODO

* Image Editor
* Sound Editor
* Model Editor
* Image Processing with OpenCV
* DICOM, STL, PDB file support
* GroundControl support
* Makefile support
* Emulator support
* CSV support and Keras panel
* GGPT Panel
* Git Support

![frame](assets/code-dicom.png)
![frame](assets/code-image.png)
![frame](assets/code-stl.png)
![frame](assets/code-pdb.png)

# License

Move to [here](https://github.com/JackCampbell/CodeEd/blob/master/LICENSE)

# Contact

* B. Firat OZDEMIR - Software Engineer / Mail: b.firat.ozdemir@gmail.com

---
> © 2021. B. Firat OZDEMIR. All rights reserved.




