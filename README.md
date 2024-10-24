https://llvm.org/docs/tutorial/MyFirstLanguageFrontend/index.html

This tutorial introduces the simple “Kaleidoscope” language, building it iteratively over the course of several chapters, showing how it is built over time. This lets us cover a range of language design and LLVM-specific ideas, showing and explaining the code for it all along the way, and reduces the overwhelming amount of details up front. We strongly encourage that you work with this code - make a copy and hack it up and experiment.

This tutorial is illustrated with a toy language called “Kaleidoscope” (derived from “meaning beautiful, form, and view”). Kaleidoscope is a procedural language that allows you to define functions, use conditionals, math, etc. Over the course of the tutorial, we’ll extend Kaleidoscope to support the if/then/else construct, a for loop, user defined operators, JIT compilation with a simple command line interface, debug info, etc.

## Compiling and Running C++ Files

### Compile a C++ file:


Add to Chat⇧⌘L
Add to Composer⌘I
⌘K to generate a command
For the code present, we get this error:
```
expected a ';'
```
How can I resolve this? If you propose a fix, please make it concise.

To resolve the error "expected a ';'", you need to add semicolons at the end of the variable declarations. Here's the concise fix:
lexer.c
tok_number
This change adds the missing semicolons at the end of each line. In C++, statements typically end with a semicolon, including variable declarations.
add what I will need to run c++ files and add commands to readmes so I know what commands I need to run c++ files

To run C++ files, you'll need to set up a C++ development environment. Here's what you'll need and the commands to compile and run C++ files:
Install a C++ compiler:
On Windows: Install MinGW or Visual Studio
On macOS: Install Xcode Command Line Tools
On Linux: Install GCC (usually pre-installed)
2. Add the following to your README.md file:
## Compiling and Running C++ Files

### Compile a C++ file:
g++ -std=c++11 your_file.cpp -o output_name

### Run the compiled program:
./output_name

# C++ Project

This project contains C++ source files. To compile and run these files, you'll need a C++ compiler installed on your system.

## Prerequisites

1. Install a C++ compiler:
   - On Windows: Install MinGW or Visual Studio
   - On macOS: Install Xcode Command Line Tools
   - On Linux: Install GCC (usually pre-installed on most distributions)

2. Ensure the compiler is in your system's PATH.

## Compiling and Running C++ Files

To compile and run a C++ file, use the following commands in your terminal:

1. Compile the file:
   ```
   g++ -o output_name source_file.cpp
   ```

2. Run the compiled program:
   ```
   ./output_name
   ```

For example, to compile and run `lexer.cpp`:
