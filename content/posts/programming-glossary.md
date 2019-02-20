---
title: "A (Mostly) Jargon-Free Glossary of Programming Terms"
date: 2019-02-18T20:25:05-08:00
lastmod: 2019-02-19
---

# Table of contents
[A](#A) [C](#C) [D](#D) [F](#F) [H](#H) [L](#L) [M](#M) [N](#N) [R](#R) [S](#S) [V](#V)

# <a name="A"></a> A
- <a name="abstraction"></a> abstraction: A way of thinking about a problem that makes it easier
  to reason about. For example, say we want to write a program that fetches some data from a
  server. We might write a function that *abstracts* away the nitty-gritty details of actually
  making the request, handling errors in case the server is down, etc. Once we have implemented
  this function (and assuming there are no bugs), we can then use the function wherever we want
  to in the rest of the program to get data from the server without having to worry each time about
  the details of how it works under the hood.

- address: A location in [memory](#memory). Most [high-level
  languages](#high-level-programming-language) [abstract](#abstraction) the concept of memory
  addresses away from the programmer.

# <a name="B"></a> B
- branch: A splitting off from a common source of code (either another branch, or the
  [master](#master) branch) that allows you to work on a feature without affecting the progress of
  other parallel branches. See also: [version control](#version-control).

# <a name="C"></a> C
- <a name="client"></a> client: A computer (or, depending on the context, a program) that
  requests data from a [server](#server).

- <a name="commit"></a> commit: In Git, a logical collection of changes that can be annotated with a
  message to describe what the changes are and the reasoning behind them. The commit is the main
  object that Git allows you to manipulate---you can reorder commits, change their contents, move
  them between branches, and more.

# <a name="D"></a> D
- <a name="directory"></a> directory: A grouping of files on the filesystem. Synonymous with
  *folder*. By placing files and other directories into directories, we form a hierarchy of files on
  the filesystem that makes it easier to locate and reference files.

# <a name="F"></a> F
- <a name="filesystem"></a> filesystem: A way of representing and managing how data on a computer
  is stored and accessed. Filesystems provide things like files, [directories](#directory), and
  links (also called aliases in macOS, shortcuts in Windows) to help users organize and access
  data on a computer. Typically, we use this term to refer to files stored on the hard drive, but
  filesystems can, among other things, also be for storage devices that networked (i.e. not in
  the same computer).

- <a name="function"></a> function: A basic unit of computation that does something useful,
  possibly using one or more input parameters and returning one (or many, depending on the
  programming language) values. Often times, we group logically related computations together in
  one function. See also: [abstraction](#abstraction).

# <a name="H"></a> H
- <a name="hard-drive"></a> hard drive: Also called *hard disk*, *hard disk drive*, *HDD*. A
  mechanical device consisting of magnetic platters (literally a metal *disk*) that store data
  and an arm with a magnetic head that reads and writes data to the platters. Reading and writing
  data to disk is slow compared to reading and writing data to RAM, but hard drives can store much
  more data for less cost and can keep this data even after the computer is powered off.

  ![Hard drive](/glossary/hard-drive.jpg)

- <a name="high-level-programming-language"></a> high-level programming language: A programming
  language that [*abstracts*](#abstraction) away from the programmer more details about how the
  computer executes a program. Typically, high-level languages are easier to use and understand,
  but the tradeoff is usually lower performance (slower programs) or the inability to do more
  complex things that the language does not allow, whether by design or not. The definition of
  what programming languages count as "high-level" varies depending on the period of history
  we're talking about, or even who you talk to, but most people will not argue that languages
  like Python, R, and shell script are high-level. See also: [low-level programming
  language](#low-level-programming-language).

# <a name="L"></a> L
- <a name="local"></a> local: Refers to something on the same computer, as compared to something on
  a different computer ([remote](#remote)). See also: [network](#network).

- <a name="low-level-programming-language"></a> low-level programming language: A programming
  language that [*abstracts*](#abstraction) away from the programmer fewer details about how the
  computer executes a program. Examples of low-level languages include C and assembly. See also:
  [high-level programming language](#high-level-programming-language).

# <a name="M"></a> M
- <a name="master"></a> master: The name commonly given to the main, canonical branch of
  development. A common action to start working on a feature might be to make a new *development*
  (or *dev*) branch from *master*. Once you are done with development on that branch, you
  [merge](#merge) it back into *master*.

- <a name="memory"></a> memory: Computers have hardware that allow them to store data for some
  period of time. Depending on the type of memory, data can be kept in memory for as long as it
  is receiving power (*volatile* memory), or it can be kept even after it is powered down
  (*non-volatile* memory). In most contexts, the term *memory* refers to random access memory
  (RAM). When you run a program, it is first loaded into RAM before it is executed so that the
  CPU can read it.

- <a name="merge"></a> merge: The act of combining two branches back into one. Once your work on a
  feature in a separate branch is complete, you usually *merge* your feature branch into *master*.

- <a name="metadata"></a> metadata: Literally, data about data. One example might be metadata for
  files: the file itself is the actual data, and the time it was last modified, its size, etc. would
  be the metadata.

# <a name="N"></a> N
- <a name="network"></a> network: Many mutually connected computers that can talk to each other. The
  Internet is a vast *network* of computers located around the world that uses the Internet
  protocol (IP) suite to communicate.

# <a name="P"></a> P
- <a name="pull"></a> pull: In Git, the act of pulling retrieves work from other developers (or
  even yourself) from a [*remote*](#remote) to your local machine. This allows you to work on the
  code locally.

- <a name="push"></a> push: In Git, the act of pushing publishes your work to a [remote](#remote).
  This makes it visible to other developers and also saves a copy of your work to the *remote*.

# <a name="R"></a> R
- <a name="remote"></a> remote: Refers to something on a separate computer, as compared to something
  [local](#local). In Git, a *remote* repository (simply called a *remote*) is a repository
  located on another computer. You can collaborate with other developers by [pushing](#push) your
  work to and [pulling](#pull) other people's work from a common remote. In Git, the main remote
  is usually named *origin* by convention.

- <a name="repository"></a> repository: Also *repo* for short. A collection of files and
  associated [metadata](#metadata) that help developers keep track of code and the history of
  changes made to that code. Closely tied to the concept of [version control](#version-control).

# <a name="S"></a> S
- <a name="server"></a> server: A computer (or, depending on the context, a program) connected to
  a network that can respond to requests for data from clients. When we visit websites on the
  Internet, our web browser (Chrome, Firefox, Safari, etc.) is a client that requests data from a
  server (e.g. Google servers, Facebook servers), which then respond to our browser with data
  (HTML, CSS, JavaScript). Our web browser then *renders* this content into something that it can
  draw on the computer screen as a graphical representation of the data provided by the
  server---the actual webpage.

- <a name="source-code"></a> source code: Also *source* for short. The file containing the actual
  text of code (hence the name *source*) that we write. For example, if we are writing Python, we
  would put our code in `.py` files, which would be our *source* files.

# <a name="V"></a> V
- <a name="version-control"></a> version control: A system to manage changes to source code.
  Especially important when working with multiple developers. Version control allows us to keep
  track of who made changes to what files when, to append notes to changes so that we can explain
  why we made those changes, and the ability to roll back changes if necessary. Popular *version
  control systems* include Git, Mercurial, and Perforce.
