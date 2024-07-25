# Get Start with OCaml

> TL;DR: What is, Installation, Setup support utility.

## What is OCaml ?

A general-purpose programming language with system-level access, multiple paradigm but functional is 
the first-class citizen that evaluated by compilation into native binary executable, bytecode or javascript.

## Installation

OCaml work best in Unix-like environment, currently the plan to support Windows natively still in progress such DKML (I already tried but
immature) other way such WSL or plain Cygwin maybe best option for now.

[You could find the tuts from it officially here](https://ocaml.org/install).

If you use Windows, use WSL (version 1 to safe RAM and use Debian for better integration with OPAM) 
and connect it with VSCode remote host.

## Setup Support

Installing OCaml just come with compiler and it standard library, which too masochist, you need to 
put some library to conviniently to stuff with OCaml. 

- [Setup Your Editor](https://ocaml.org/docs/set-up-editor), seriously this improve you development experience such code highlight, type notation, so forth.

And install this various library in order to fill your need (run `opam install <package name>`, dont write the angle bracket):

|Package|What its purpose|
|--|--|
| `dune` | project manager/build tool for your codebases such `npm`, `rubygems` |
| `utop` | better REPL interface |
| `cmdliner` | for making quite serious CLI programs such parse command line, generate manpages for it (I found quite usefull) |
| `lwt` | multi-threading  |
| `alcotest` | colorful unit testing  |
| `menhir` | parse something with Context-free grammar |
| `tyxml` | HTML/XML/SVG swiss army knife  |
| `lambdasoup` | HTML parse and scrape  |

My recommendation : `dune` for manage alot of code and `utop` to test code interactively.
