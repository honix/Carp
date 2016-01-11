# Carp

<img src="https://github.com/eriksvedang/Carp/blob/master/img/temp_logo2.jpg" alt="Logo" align="right" />

Carp is a small programming language designed to work well for interactive and performance sensitive use cases like games, sound synthesis and visualizations.

The key features of Carp are the following:

* No garbage collection or runtime system, all memory management is deterministic and compiled into the final library or executable
* Static, 100% inferred type system that enables very fast code execution and fewer runtime errors
* Dynamic code loading and live evaluation allows interactive (REPL-driven) development of your program
* No hidden performance penalties, everything that can slow down your program is explicit and visible in the code
* Ownership system that enables a pure functional programming style while still using mutation to get fast updating of data structures
* Very good integration with C libraries

## The Language
Carp is heavily inspired by languages like Clojure, Scheme, Haskell, ML and Rust. Here's a sample program:

```clojure
(defn main ()
  (println "Hello!"))
```

## The Compiler
Carp is very tightly integrated with it's compiler which itself is written in a dynamic version of Carp (the dynamic version is implemented in C). To compile or work on a Carp program you start the Carp compiler system which puts you in the compiler REPL. Everything you want to do with your program can be controlled from here.

(C) Erik Svedäng 2015 - 2016
