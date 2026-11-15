<div align="center">

<a href="https://42.fr/"><img src="https://raw.githubusercontent.com/doooriian/42-Badges/main/badges/minishellm.png" alt="minishell 42 badge" width="125" /></a>

# minishell

**42 School project · Unix shell implementation**

<img src="https://img.shields.io/badge/42_Project-C%20%7C%20Unix%20shell-0F766E?style=flat-square" alt="minishell technology" />
<img src="https://img.shields.io/badge/Documentation-Project_Overview-334155?style=flat-square" alt="Project documentation" />

</div>

## 🔎 Overview

A simplified UNIX command interpreter that parses commands, executes processes, and manages redirections and pipelines.

## ✨ Features

- Tokenize and parse shell commands
- Run external executables and common built-in commands
- Handle pipes, input/output redirections, and heredocs
- Expand environment variables and handle interactive signals

## 🧩 Technical approach

The codebase separates tokenization, parsing, execution, and built-ins. It uses POSIX process and file descriptor primitives and GNU Readline for interactive input.

> **Tech stack** · C · POSIX · GNU Readline · Make.

## 🚀 Build and usage

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

## 🧪 Verification

Build in the documented environment, exercise normal scenarios and edge cases, and compare actual behaviour with the expected output. No automated CI test suite is included in this repository.

## ⚠️ Notes and limitations

This is an educational shell rather than a full Bash replacement. The repository is a GitHub fork; project authorship and individual responsibilities should be credited according to the original contributors.

---

<div align="center">

<sub>Part of the <a href="https://42.fr/">42 curriculum</a> · <a href="https://github.com/doooriian">Back to my GitHub profile</a></sub>

</div>
