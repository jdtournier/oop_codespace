# Getting started to programming with C++
### Week 1, session 1

# Teaching team

## Module leads & lecturers

| ![donald](.assets/donald.jpg) | ![michela](.assets/michela.jpg) | ![toby](.assets/toby.jpg) |
| :---: | :---: | :---: |
| [J-Donald Tournier](mailto:jacques-donald.tournier@kcl.ac.uk) | [Michela Antonelli](mailto:michela.antonelli@kcl.ac.uk) | [Tobias Wood](mailto:tobias.wood@kcl.ac.uk) |

## Teaching assistants

| ![nashira](.assets/nashira.jpg) | ![adriana](.assets/adriana.jpg) | ![hasara](.assets/hasara.jpg) | ![?](.assets/.jpg) |
| :---: | :---: | :---: | :---: |
| [Nashira Baena](mailto:paloma.rodriguez_baena@kcl.ac.uk) | [Adriana Namour](mailto:adriana.namour@kcl.ac.uk) | [Dewmini Hasara Wickremasinghe](mailto:dewmini.wickremasinghe@kcl.ac.uk) | |
| ![abhijit](.assets/abhijit.jpg) | ![charel](.assets/charel.jpg) | ![yovin](.assets/yovin.jpg) | ![jakub](.assets/jakub.jpg) |
| [Abhijit Adhikary](mailto:abhijit.adhikary@kcl.ac.uk) | [Charel Mangama Sindzi](mailto:charel.mangama_sindzi@kcl.ac.uk) | [Yovin Yahathugoda](mailto:yovin.yahathugoda@kcl.ac.uk) | [Jakub Grzelak](mailto:jakub.grzelak@kcl.ac.uk) |


# Course overview

## Objectives

This course is an introduction to object-oriented programming using C++.

It will provide you with an understanding of:
- the Unix command-line
- how to handle and manage files and commands in a Unix environments
- the basics of programming using C++
- the basics of the object-oriented programming paradigm
- how to manage and process complex data structures

Where possible, the course aims to provide you with transferable skills that can be
applied in other situations. For many of you, these skills will prove valuable
for your final project &ndash; *even if you don't use C++!*

We will initially cover a lot of topics quickly and superficially. The point is
to rapidly get to the point where you can start writing your own code. Not
everything will immediately make sense - but hang in there: with a bit of
practice, it will all become clear!

## Structure

This is a 10 week course, with 2-hour hands-on practicals twice a week. For
each session, you are expected to read the preliminary reading material
provided, so that you can immediately start working on the worksheet within
each hands-on session. 

The intention is to maximise the amount of practice time, so that you can gain
as much experience with programming as possible. **There is no substitute for
practice:** this is the only way to become proficient in programming (C++ or
otherwise).

## Assessment

There are two assessments on this module, both performed in-person in the
Student Computer Rooms. You will be required to write and/or modify 
C++ programs using the development environment introduced on this course. 
We will go through practice versions of each of these in the sessions to make
sure everyone is familiar with the procedure and requirements. You are all
**strongly** advised to attend these sessions in particular!

- Week 5: practice for first assessment
- Week 6: first assessment (30%)
- Week 9: practice for second assessment
- Revision week: second assessment (70%)

## How to make the most of this course

Learning to program can only be done through experience
- please make every effort to **attend all the tutorials!**
- don't hesitate to ask if anything is unclear or you need any help
- avoid the temptation to use AI tools!
- go through all the exercises
- search online for more examples and explanations!
  - but bear in mind that online sources may use concepts we have
    deliberately left out of the course, or rely on a different version of the
    C++ standard!

## External reference material

We encourage you to read up on difficult and/or important topics. There are
many very good sources of information available to you, including tutorials,
internet forums, and books (many of them available online). Be careful though,
you will find many different opinions on various topics, and it can be
difficult to work out what is good advice &ndash; you will need to exercise
your judgement!

Good online resources include:

- [learncpp](https://www.learncpp.com/cpp-tutorial/introduction-to-cplusplus/): a great tutorial, accessible and up to date
- [cppreference.com](http://en.cppreference.com/w/cpp): very thorough C++ reference, up to date and correct, but not easy for beginners
- [C++ FAQ](https://isocpp.org/faq): great resource with answers to general or specific questions

Other online sources (not as authoritative as the above):

- [geeksforgeeks.org](https://www.geeksforgeeks.org/c-plus-plus/): great as a quick introduction to key concepts, but can often be too simplistic
- [cplusplus.com](http://www.cplusplus.com/): C++ tutorial and reference, a little out of date

# What is C++?

C++ is a widely-used general-purpose programming language, ranked second on the
[TIOBE programming community index](https://www.tiobe.com/tiobe-index/) (after
[Python](https://www.python.org/)). It is used for high-performance and/or
resource-constrained software, and can be used for a wide range of
applications: embedded systems, operating systems, desktop applications,
telecoms infrastructure, ...

C++ was first released in 1985 by Bjarne Stroustrup as an extension to the [C
language](https://en.wikipedia.org/wiki/C_%28programming_language%29). It was
first standardised by the [International Organization for Standardization
(ISO)](https://www.iso.org/) in 1998, and there have been many versions of the
standard since (bold denotes fundamental changes): - **C++98**, C++03, **C++11**, C++14, C++17, **C++20**, C++23, **C++26** (under development)

On this course, we will be using the **C++20 version of the standard**

Specific features of C++:
- It supports [Object-Oriented Programming (OOP)](https://www.geeksforgeeks.org/introduction-of-object-oriented-programming/), as well as [generic](https://www.geeksforgeeks.org/generics-in-c/) and [functional programming](https://www.geeksforgeeks.org/functional-programming-paradigm/)
- It is a [compiled
  language](https://www.geeksforgeeks.org/difference-between-compiled-and-interpreted-language/):
  the code you write must be *compiled* to native [machine
  instructions](https://www.geeksforgeeks.org/computer-organization-architecture/machine-instructions/)
  before execution. This should in theory provides the highest performance,
  avoiding the overhead of interpreting the instructions at runtime. It also
  provides an opportunity to detect certain classes of errors at an earlier
  stage, before any attempt is made at running the program. It also allows the
  compiler to apply various optimisation techniques to produce more efficient
  code. However, the compile cycle can be lengthy, slowing down the development
  process.
- It uses [static
  typing](https://www.geeksforgeeks.org/type-systemsdynamic-typing-static-typing-duck-typing/):
  data types are known and checked at compile-time, not runtime. This ensures
  the code is well-defined and allows the compiler to catch many types of
  errors at compile time, before even trying to run the code. It does however
  require more discipline when writing the code. 


## What this course will *not* cover

Bear in mind that this is an *introductory* course to C++ and Object-Oriented
Programming. It is not possible to cover all of the many features, idioms,
design patterns and other idiosyncracies of the language within a short 10 week
course. This course will therefore only cover the basics of the language, and
focus on the minimum required to write small but effective programs.

Of the topics not covered on this course, the most notable is manual memory
management; this would be considered fundamental in many other courses.
However, the general recommendation for modern C++ is to avoid manually
managing your own memory if possible, given how easy it is to get it wrong and
introduce potentially hard-to-find errors in your programs (which can often
also have serious security implications!). Bear in mind that you may need to
learn about this (and other topics) if you wish to become profficient in C++.


# The development environment

## The IDE: integrated development environment

Most programmers will use an [integrated development
environment](https://www.geeksforgeeks.org/blogs/what-is-ide/) to write and
test their code. Most IDEs provide an interface including an editor window,
utilities for file management (including revision control), for compiling and
running code, and for debugging, and access to a terminal, amongst many other
features.

There are many IDEs available, with some being more suited to
different languages. On this course, we will use the popular [Visual Studio
Code (VSCode)](https://code.visualstudio.com/) IDE. 

Setting up your development environment can be tricky, and is often the biggest
hurdle facing begginers. To avoid any issues around installation, we will use
[GitHub](https://github.com/)'s online [CodeSpaces
service](https://github.com/features/codespaces), which provides a running
instance of VSCode hosted on the cloud, and accessible through any web browser.
This means you will be able to log onto your own codespace from anywhere, and
pick up where you left off, without having to set anything up on your own
computer.

## The terminal

On this course, we will use the *terminal* to compile and run the code. While
it is possible to write C++ code without using the terminal, this severely
limits how you can use your programs. In practice, the terminal provides a much
more flexible and powerful way to run your programs and interact with them
&ndash; especially as a beginner. More generally, using a terminal is a very
useful skill and will prove useful in many other contexts, for example when
undertaking your final-year projects &ndash; it really is worth spending some
time getting familiar with it! 

The terminal provides access to the
[command-line](https://www.geeksforgeeks.org/operating-systems/what-is-command-line-interface-cli/),
which is a text-based interface used to interact with a computer's operating
system. It allows you to type in commands for the system to execute, and to view any
output these commands produce. It is also known as the *command-line terminal*,
*command-line interface (CLI)*, *console*, or *shell*. 

> 🎓 In reality, the command-line interface consists of two interacting parts: 
> - the *terminal* itself is responsible for displaying the text to the user,
>   and taking input from the user. It is not responsible for taking any
>   further action; it merely acts as an intermediary between the user and the *shell*.
> - the *shell* or *command-interpreter* is a program that interact with the
>   terminal, and processes and produces text. It is responsible for
>   *interpreting* the user's input, and running any programs as instructed. 
> 
> In essence, the *shell* is the 'brains' of the command-line interface, with the
> *terminal* itself providing the front end (a graphical interface that the user
> can interact with).
> 
> There are [many different terminals available](https://en.wikipedia.org/wiki/List_of_terminal_emulators), and
> [many different shells available](https://en.wikipedia.org/wiki/List_of_command-line_interpreters),
> which can all be used in different combinations. 


On this course, we will rely on the [terminal provided by
VSCode](https://code.visualstudio.com/docs/terminal/getting-started), and the
widely-used [Bourne-Again shell
(BASH)](https://en.wikipedia.org/wiki/Bash_%28Unix_shell%29), which is the
default on most Unix-based operating systems. The instructions on this course
are specific to the BASH shell, and will work in most Unix environments
(including macOS).

> 💡 Familiarity with the terminal and the command-line will help greatly 
with your performance on this module, and enhance your ability to handle
computers in other contexts (not just for C++!). It is strongly recommended
that you take the time to experiment with the terminal and practice until you
feel confident. We strongly encourage you to go through our [Introduction to
the Unix command-line](https://command-line-tutorial.reagqdthedocs.io/)
tutorial, in addition to this document and the associated worksheet.

### The command prompt

When started, the shell will show a *prompt*, and wait for you to enter
commands.  The prompt will (typically) take the form:
```
user@hostname:folder $
```

where:
- `user` is your current username
- `hostname` is the name of the computer this session is currently running on
- `folder` is the folder you are currently operating in (the _current working
  directory_)

> 💡 The `~` symbol is used as a shorthand for your home folder

### Anatomy of a command

When typing in a command on the terminal, the first 'word' is the command name,
and will typically correspond to a file on your computer that contains the code
to be executed &ndash; which will often be your own program!

Subsequent 'words' correspond to *arguments*, and will be passed to the command
when it is executed. This is the primary mechanism by which we can interact
with our programs: it allows us to specify which files are to be processed,
using what parameters, or any other information necessary for our program to
perform the actions we expect it to do.

By convention, commands often treat certain arguments as *options*. Such
*options* typically start with a single or double dash, following by a single
letter or longer (and more descriptive word) respectively. For example, many
commands will accept an option such as `-h` or `--help` (and may accept
either), which results in the command printing a brief help page. 

A command may be able to run without any arguments, or it may refuse to run
without them &ndash; this depends on what the command is designed to do, and
how the original developers intended it to be used! We will see how to interact
with command-line arguments for our own programs in due course.

## Files and folders

A crucial aspect of working with the command-line is working with files and
folders. We will often need to specify which file our program is supposed to
process, or exactly where the command we wish to run is located. This requires
an understanding of how data are stored in *files* and organised in *folders*
(officially called *directories* in computing), and how to specify a file or
folder on the command-line. 

If you are unfamiliar with the concept of files and folders, [here is a
very good overview](https://www.hendrik-erz.de/post/understanding-files-and-folders-a-primer)
that you are strongly encouraged to read. 

### The working directory

When a program or command is invoked, it will start up within its own 
[working directory](https://en.wikipedia.org/wiki/Working_directory): this is
the folder where the command is running. When invoked from the terminal, your
commands will typically start in the terminal's current working directory.
On most systems, the current working directory is displayed as part of the
command prompt, and can be queried using the `pwd` (print working directory)
command. 

The working directory is important since your program can refer to
the files and folder in its working directory using their name &ndash; no need
to also specify which folder they might stored in. By running your program
within the directory (folder) that contains the data to be processed, it is
simple to specify which files your program needs to access.

### Relative path

In reality, when specifying files in the current working directory, we are
providing the *relative path* to the file: this is the location of the file
*relative* to the program's current working directory. If the file to be
processed was located within a subfolder in the current working directory, we
could provide its location as (for example): `subfolder/data.txt` (assuming we
mean the file `data.txt` in the folder `subfolder`, which is in the current
working directory). Note the use of the forward slash (`/`) as the delimiter
(this is the Unix convention). This is an example of a *relative path*: we
provide the *path* to the file, starting from the current working directory. 

We can also refer to files *outside* of the current working directory using the
special name `..`: this refers to the *parent* of the current folder. For
example, `../other_folder/data.txt` refers to a file called `data.txt`, located
within a folder called `other_folder`, which is itself located alongside (but
not within) the current working directory.

### Absolute path

When referring to files via their relative path, the interpretation is always
dependent on the current working directory. This is not always appropriate,
sometimes we need to be able to unambiguously specify *exactly* which file we
mean. For this, we can use the *absolute path*, which is the path to the file
starting from the *root* of the filesystem, denoted by a leading forward slash
(`/`). For example, the file `/home/student/subfolder/data.txt` is located
within the folders shown, *irrespective* of the current working directory. 

### Special filenames

A few filenames have special significance, and you should learn to use them, or
at least know of them. These are:

- **`~`:** shorthand for your home folder. 
- **`.`:** the current directory. 
- **`..`:** the *parent* of the current directory. 

These can all be used when specifying file paths, and can be useful in many
contexts. For example, assuming your working directory is
`/workspaces/oop_codespace/my_project`:

- `ls ..`  <br> 
  list the contents of the parent of the current working directory
  (i.e. `/workspaces/oop_codespace`)
- `ls ../data` <br> 
  list the contents of the folder `data` that resides alongside the
  current working directory (i.e. the `/workspaces/oop_codespace/data` folder)
- `cp ../data/subject1.txt .` <br> 
  copy the file `subject1.txt` that resides in the
  `data` folder alongside the current working directory (i.e. the file
  `/workspaces/oop_codespace/data/subject1.txt`) into the current folder.

### Navigating the filesystem

Within the terminal, we can inspect the contents of the current working directory
using the `ls` command. We can also use that command to display any other
folder by providing its path as an argument to `ls`.

We can move around the filesystem by changing the terminal's current working
directory. This is done using the `cd` (change directory) command, providing
the location of the folder to move to as the command argument, either as a
relative or absolute path. 

For example, `cd subfolder` changes the terminal's working directory to
`subfolder`, relative to the current folder (assuming such a folder exists).

### Essential commands

To make effective use of the terminal, there are a few essential commands to
know about:

- **[pwd](https://www.geeksforgeeks.org/linux-unix/pwd-command-in-linux-with-examples/):**
  print the current working directory
- **[ls](https://www.geeksforgeeks.org/linux-unix/ls-command-in-linux/):** list
  files and folders in the current working directory, or in the location
  specified as the (optional) argument
- **[cd](https://www.geeksforgeeks.org/linux-unix/cd-command-in-linux-with-examples/):**
  change the current working directory
- **[mkdir](https://www.geeksforgeeks.org/linux-unix/mkdir-command-in-linux-with-examples/):**
  create a new directory (folder)
- **[rmdir](https://www.geeksforgeeks.org/linux-unix/rmdir-command-in-linux-with-examples/):**
  remove an empty directory 
- **[cp](https://www.geeksforgeeks.org/linux-unix/cp-command-linux-examples/):**
  copy files or folders
- **[mv](https://www.geeksforgeeks.org/linux-unix/mv-command-linux-examples/):**
  move files or folders to a different location, and/or rename them
- **[rm](https://www.geeksforgeeks.org/linux-unix/rm-command-linux-examples/):**
  remove files (and optionally entire folders)


# Programming in C++

Writing a program in C++ involves the following steps:

1. **Create or modify the text file(s) containing our C++ code.**<br>
   C++ files will normally have the suffix `.cpp`. To write the code, we will
   need to use a suitable [text editor](https://en.wikipedia.org/wiki/Text_editor), 
   designed to handle [plain text](https://en.wikipedia.org/wiki/Plain_text)
   documents (word processing software such as Microsoft Word is *not*
   appropriate!). There are 
   [plenty of editors](https://en.wikipedia.org/wiki/List_of_text_editors)
   available, but on this course we will use the editor provided as part of
   VSCode.

2. **Compile our code.**<br>
   This involves invoking the compiler on our code
   file(s) so that it can translate our C++ human-readable code into binary
   [machine instructions](https://www.geeksforgeeks.org/computer-organization-architecture/machine-instructions/).
   The [compiler](https://www.geeksforgeeks.org/compiler-design/introduction-to-compilers/)
   is a complex set of programs that will check our code is valid,
   convert it into some internal reprensentation, [perform various optimisations](https://en.wikipedia.org/wiki/Optimizing_compiler) as
   appropriate, convert this to [assembly
   language](https://en.wikipedia.org/wiki/Assembly_language), and finally convert
   this into native binary [machine
   code](https://en.wikipedia.org/wiki/Machine_code) instructions. The result is
   an [executable file](https://en.wikipedia.org/wiki/Executable), which
   contain code that the CPU on your computer can execute directly.

3. **Invoke the resulting executable.**<br>
   We can now run the executable file produced by the compilation step, test it,
   and (most of the time) go back to step 1 and modify our C++ program as
   necessary. On this course, we will invoke the programs we write on the
   terminal, which will allow us to provide [command-line
   arguments](https://en.wikipedia.org/wiki/Command-line_interface#Arguments) to
   the program, and interact with it through its [standard input and output
   streams](https://en.wikipedia.org/wiki/Standard_streams)



## Our first C++ program: Hello World

In the worksheet, we will go through the process of writing our first program:
[Hello World](https://en.wikipedia.org/wiki/%22Hello,_World!%22_program). This
is what the C++ code looks like:


```cpp
#include <iostream>

int main ()
{
  std::cout << "Hello World\n";
  return 0;
}
```

This is a very simple program: its only action is to print the words `Hello
World` on the terminal. Nonetheless, this already illustrates many important
aspects of C++. 

Please refer to the corresponding worksheet for instructions to compile and run
this program. 

## How does this program work?

Let's go through this program line-by-line to understand what it does.

### The `#include` preprocessor directive

Most programming languages have a concept of 'modules', each providing
specific functionality. The `#include` directive is how this is done in C++.
Our program needs to use `std::cout`, and this is declared in
`<iostream>`, so we need to `#include` it for the compiler to understand how to
use `std::cout`. 

> 🎓 This is true for C++ code prior to the introduction of
> [C++20 modules](https://www.geeksforgeeks.org/cpp/modules-in-cpp-20/), which
> provide an alternative mechanism to support modules. But these are not widely
> used yet, and will not be covered on this course. 

In more detail, lines beginning with a `#` symbol are so-called [preprocessor
directives](https://www.geeksforgeeks.org/c/cc-preprocessors/). The
preprocessor runs as part of the compilation process, *before* the compiler
proper. Its job is to process these directives and perform the appropriate
actions. 

The `#include` directive instructs the preprocessor to insert the contents of
the file specified into the current file at this point, before feeding the
combined output through to the compiler itself. Here, the [`<iostream>` *header*
file](https://www.geeksforgeeks.org/cpp/basic-input-output-c/) contains the
function and object declarations we need to interact with the
terminal through its [standard input and output streams](https://en.wikipedia.org/wiki/Standard_streams), 
which we need to be able to use `std::cout`.

> 💡 We will explain *header files* later in the course. 

### The `main()` function

The next line is the [declaration](https://www.geeksforgeeks.org/compiler-design/difference-between-definition-and-declaration/) of the `main()` function. The `main()` function is the [*entry
point*](https://en.wikipedia.org/wiki/Entry_point) for any program. When we
invoke our program, the system will find our executable's `main()` function and
start our program from there. 

By convention, we declare it as
[returning](https://en.wikipedia.org/wiki/Return_statement) an integer (`int`).
We'll see more about this when we cover functions in subsequent sessions.

The contents of our `main()` function are specified within the curly braces
(`{}`). The lines enclosed within these braces define the *implementation* of the
function, and constitute the
[definition](https://www.geeksforgeeks.org/compiler-design/difference-between-definition-and-declaration/) 
of our `main()` function. 

In C++, braces are used to group statements together. We will see more about
this later

Note the use of semicolons `;` to mark the end of each of these lines

These lines are individual *statements*:
- in C++, the semicolon marks the end of the statement
- technically, these statements could both be on the same line &ndash; only the
  semicolon matters

### Standard output and input/output streams

The next line feeds the
[string](https://en.wikipedia.org/wiki/String_%28computer_science%29) `"Hello World\n"` through to the program's
[standard output](https://en.wikipedia.org/wiki/Standard_streams), using the `std::cout` [C++
stream](https://www.geeksforgeeks.org/cpp/c-stream-classes-structure/) object.
The effect is to display the text "Hello World" on the terminal.

We enclose the string within inverted commas (`"`). We will cover string
handling in more detail in the next section.

Note the use of the *insertion operator*, `<<`:
- This line reads as: insert the string "Hello World" into the `std::cout` IO
  stream.

Note also the trailing `\n` *escape sequence* at the end of the string
- The backslash `\` character can be used to *escape* the normal interpretation
  of the next character
- Here, the sequence `\n` translates into the [*newline*
  character](https://en.wikipedia.org/wiki/Newline)
- See [here for a full list of escape
  sequences](https://www.geeksforgeeks.org/escape-sequence-in-c/)


### The `return` statement

Finally, we *return* from `main()`, which marks the end of our program. 

The value returned is the [exit
code](https://en.wikipedia.org/wiki/Exit_status) of our program. 
It can be queried by other programs, or by the shell, to detect any errors
during execution
- by convention, any non-zero value signals that an error occurred.
- different error codes can sometimes be used to signal different types of
  errors (though there is no convention for what different exit codes might
  mean...).


# Summary

- C++ is a compiled language: we write the code as text, and the *compiler*
  translates our code into native machine instructions, stored in the output
  *executable*.
- We typically write our C++ code within an Integrated Development Environment
  (IDE), though technically any text editor will do
- We can use the *terminal* or *command-line interface* to compile and run our
  code, and to interact with the system more generally.
- To understand how to move around the *filesystem*, locate files and provides
  them as *command-line arguments* to our programs, we need to understand the
  concept of *relative and absolute paths*.
- Every program will have at least a `main()` function: this is the *entry
  point* into the program.
- We can use `#include` statements to use additional functionality, for example
  to access the terminal.
- We can print out text to the terminal by inserting variables into the
  `std::cout` IO stream.
