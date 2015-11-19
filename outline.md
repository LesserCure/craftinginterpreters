- Warming Up
    - Introduction
        - who book is for
        - who am i
            - doodling languages in notebook
            - always fascinated
            - seemed like magic
            - iStudio
            - paternity
            - Dart
        - why learn languages?
            - in full programming career, will end up doing something related to
              language
            - good way to learn lots of techniques: recursion, trees, graphs,
              state machines, memory management, optimization
            - hard, training with weights on
            - fun
            - dispell magic
        - structure of book
        - languages used in impl
        - what's in book
        - what's not in book
        - end goal is high quality, efficient interpreter suitable for real use
        - to get there, narrow path through space, not broad survey
        - will point to alternatives to explore on own
        - learn enough to carry conversation with professional lang person
    - Your First Interpreter
        - basic phases and terminology of interpreter
        - simple stack-based language
    - Your Second Interpreter
        - intro to full language we'll be implementing
        - ebnf
- Practice (JS)
    - Read, Eval, Print, Loop
        - interpreters run from source
        - test framework
    - Scanning
        - tokens
        - whitespace
        - regex
        - comments
        - numbers
        - token value
        - strings
        - token type
        - escaping
        - errors
    - Parsing Expressions
        - ast
        - recursive descent
        - operator precedence
        - lookahead
        - top-down operator precedence parsing
    - Tree Walk Interpreting
        - evaluating operands
        - recursion
        - arithmetic
        - visitor pattern
        - values versus ast nodes for literals
        - dynamic typing and conversions
        - errors
    - Variables
        - statements
        - declaration
        - assignment
        - variable references
        - scope
        - name binding
        - undefined names
        - block scope
    - Control Flow
        - if
        - && and ||
        - while
        - for
    - Functions
        - parsing calls
        - '(' as infix operator
        - built in fns
        - user-defined fns
        - parameters and arguments
        - call stack
        - closures
        - ffi?
        - tail call optimization
- Performance (C)

principles
- each top-level section builds one interpreter starting from scratch
- since the book will be "published" online serially, the chapters should be
  ordered such that they are useful even while the book is incomplete. that
  probably means doing all of parsing for the whole grammar isn't a good idea:
  it's boring until later chapters do something with it.

- kinds of content in a chapter
  - main narrative with prose and code
  - historical context and people
  - further things to learn
  - omitted alternatives
  - exercises
  - quotation at beginning of each chapter

stuff to maybe include:

- gc
    - mark-sweep collection
    - copy collection
    - lisp2 algorithm?
    - bump-pointer allocation
    - roots
- error-handling
    - stack traces and line information
    - lexer errors
    - compile time errors
    - runtime errors
- variables
    - scopes as dictionaries
    - name binding of locals
    - variables and assignment
    - scope
- object model
    - objects as dictionaries
    - objects
    - classes
    - prototypes
    - nan tagging
    - object representation
    - symbol tables and hash tables
    - strings
    - arrays
    - hash tables (for internal use and as object in language)
    - dynamic dispatch
- syntax
    - aesthetics and usability of syntax design
    - backjumping and infinite lookahead or context-sensitive grammars
- execution
    - compiling to bytecode
    - virtual machine
    - stack based bytecode
    - register based bytecode
    - fibers and coroutines

- kinds of asides
  - historical context and people
  - further things to learn
  - omitted alternatives
  - engineering considerations: error handling, maintainability, etc.
  - design and pyschology: usability, aesthetics, popularity, learnability, etc.