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

__CodeEd__ is built on a powerful code editor and developer tools. It was originally designed for application and unit development. Since 2020, it has been developed based on user needs, focusing on low energy consumption and ease of use. Today, _it is actively used in many projects_.

![app](assets/code-main2.png)


## C/C++ Tools

This IDE application provides a number of features in the C/C++ environment.

### Auto Complete

Code completion is a feature aimed at enhancing efficiency in the software development process. This process involves taking an (incomplete) source file while determining where the user is actively editing that file. In this context, code completion suggests syntactically and semantically valid constructs that the user may find useful at that specific point in the source code. These suggestions not only accelerate the writing of code but also help ensure that users utilize the correct syntax and structures, reducing the likelihood of errors. Thus, it enables developers to work more efficiently and minimizes time lost in complex projects.


![giphy](assets/code-autocomplete1.gif)
![giphy](assets/code-autocomplete2.gif)


### Code Tip

This feature ensures that the functions within the source files of the project are called correctly and that default arguments are easily visible to the user. Additionally, when an unclosed parenthesis is encountered for a function, a small window opens to provide information about the function's parameters. This window helps developers by showing which arguments are expected, thereby accelerating the coding process and aiding in error prevention. As a result, users can create their code more effectively and make the most of the available functions.

![giphy](assets/code-calltip1.gif)

### Diagnostics

This feature instantly informs the software developer of any errors or warnings that may occur during the operation of the application. Errors are presented in a list format along with a diagnostic panel, allowing developers to quickly identify and resolve issues. This list is enriched with error codes and descriptions, enabling developers to more easily understand the root cause of the problem. Additionally, users can customize this feature in the application settings, adjusting the appearance and behavior of notifications to suit their needs. This ensures a more efficient development process overall.

![giphy](assets/code-diagnostic1.gif)

### Build Command Database

A build database comprehensively contains the arguments used for compiling files within a project. For each file in the database, details about the working directory or command line used for the compiler call can be queried, providing developers with flexibility in managing the compilation process. This structure ensures that the source files in the project are accurately translated into C/C++ language while also ensuring that all components of the project work in harmony. Consequently, developers can proactively identify potential issues they might encounter during the compilation phase and take the necessary measures to maintain the integrity of the project.

### Serialization

This feature serializes the system files associated with your projects, enabling faster translation of source files. For a more efficient compilation process, you need to add the precompiled header file to your project and activate this feature in the application settings. Whenever any changes are made, the precompiled header file is updated, resulting in the re-serialization of the system files. This process significantly reduces compilation time, allowing developers to work more quickly and enhancing the overall performance of your project.

### Indexer

This feature indexes the classes and functions found while navigating through the source files in the project in a cache environment. The indexing process enables quicker and more efficient access to the source code, allowing developers to instantly retrieve the information they need. As a result, the coding process accelerates, enabling developers to work more effectively on their projects.

![dialog](assets/code-spotlight.png)

### Code-Format

Code-formatter is a tool that automatically formats C/C++ code, allowing developers to focus on functionality rather than style issues during code reviews. In addition to making your code neat and readable, formatting your C/C++ code is crucial for enhancing the efficiency of the project process. This not only saves time for you but also for your reviewers. The CodeEd application utilizes the powerful clang-formatter API to carry out this task. Users can choose from specific available formats in the settings dialog or create their own custom format by reading the `.clang-format` file within the project. This ensures consistent styling across every project, thereby improving code quality.

![giphy](assets/code-format.gif)

### Debug

In general, a debugger is a computer program that assists developers in testing and debugging other programs. `LLDB` and `GDB` are two of the most popular and powerful debuggers available. CodeEd integrates the `LLDB API`, providing users with comprehensive debugging capabilities. This integration allows developers to identify and resolve issues in their code more quickly, thereby accelerating their development processes. The debugging process is crucial for enhancing software quality and improving user experience.

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

This feature allows you to test the project you are working on after it has been compiled, providing significant convenience in your software development process. The testing process is initiated by the configuration specified by the user; this enables developers to quickly evaluate their projects under different scenarios. Additionally, the configuration arguments and the target file specified by the macro remain consistent, even if the project is moved, thereby providing flexibility to test the project in various environments.

![giphy](assets/code-process.gif)


## Design And Resource

This feature supports application development and user-friendly desktop form design with the `wxWidgets` environment, providing developers with a powerful platform. The flexibility and functionality offered by `wxWidgets` allow users to create attractive and effective interfaces. This IDE has been developed using these powerful tools, making the application development process more efficient and enjoyable for users.

![frame](assets/code-resource.png)
![frame](assets/code-design.png)

## CMake Support

CMake support allows you to build, automate, test, package and install software in a multi-platform environment.

![frame](assets/code-cmake.png)

## Javascript

Provides support for nodejs projects with a Javascript runtime environment. Provides autocompletion and function signature at coding time.

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
* `Language Server Protocol` (LSP) support. (experimental)


![frame2](assets/code-sqlite3.png) ![frame2](assets/code-hex.png)

# License

Move to [here](https://github.com/JackCampbell/CodeEd/blob/master/LICENSE)

# Contact

---

| ------------------------------------------ | ------------------------------------------------------ | ----------------------------------------- |
| [E-mail](mailto:b.firat.ozdemir@gmail.com) | [Linkedin](https://www.linkedin.com/in/bfiratozdemir/) | [Github](https://github.com/JackCampbell) |


> © 2021. B. Firat OZDEMIR. All rights reserved.


