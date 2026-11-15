# minishell

> **42 School project** · C · Processes · Shell

A simplified UNIX command interpreter that parses commands, executes processes, and manages redirections and pipelines.

## Overview

A simplified UNIX command interpreter that parses commands, executes processes, and manages redirections and pipelines.

## Features

- Tokenize and parse shell commands
- Run external executables and common built-in commands
- Handle pipes, input/output redirections, and heredocs
- Expand environment variables and handle interactive signals

## Technical approach

The codebase separates tokenization, parsing, execution, and built-ins. It uses POSIX process and file descriptor primitives and GNU Readline for interactive input.

**Stack:** C · POSIX · GNU Readline · Make.

## Build and usage

**Platform:** UNIX-like environment with GNU Readline development headers and library.

```bash
git clone https://github.com/doooriian/minishell.git
cd minishell
make
./minishell
```

Inside the shell:

```bash
pwd
export NAME=42
echo $NAME
ls -la | grep README
exit
```

## Verification

Build in the documented environment, exercise normal scenarios and edge cases, and compare actual behaviour with the expected output. No automated CI test suite is included in this repository.

## Notes and limitations

This is an educational shell rather than a full Bash replacement. The repository is a GitHub fork; project authorship and individual responsibilities should be credited according to the original contributors.

---

Part of the [42 curriculum](https://42.fr/). Explore the other projects on [my GitHub profile](https://github.com/doooriian).
