<div align="center">

<a href="https://42.fr/"><img src="https://raw.githubusercontent.com/doooriian/42-Badges/main/badges/minishellm.png" width="125" alt="minishell 42 project badge" /></a>

# minishell

**Unix shell and process management**

<img src="https://img.shields.io/badge/42%20School-Project-0F766E?style=flat-square" alt="42 School project" />

</div>

---

## 🔎 Overview

**Minishell** is a 42 School project that recreates a simplified version of a UNIX shell.  
This project challenges your understanding of **process creation**, **pipes**, **redirections**, **signals**, and **environment management** — all core concepts of systems programming in C.

The goal? Build a fully functional shell that mimics Bash-like behavior while adhering to 42’s strict coding standards.

---

## ✨ Key Features

- **Command Execution**  
  Executes commands using `fork`, `execve`, and `waitpid`.

- **Built-in Commands**  
  Supports the main shell built-ins:
  - `echo` — Displays text.
  - `cd` — Changes directory.
  - `pwd` — Prints current working directory.
  - `export` / `unset` — Manages environment variables.
  - `env` — Displays environment variables.
  - `exit` — Exits the shell.

- **Pipes & Redirections**  
  Handles operators like:
  - `|` — Command chaining.
  - `<`, `>` — Input/output redirection.
  - `>>` — Append output.
  - `<<` — Heredoc functionality.

- **Signal Handling**  
  Correctly manages `SIGINT` (Ctrl+C), `SIGQUIT` (Ctrl+\), and ignores signals in child processes for Bash-like behavior.

- **Environment Variable Expansion**  
  Expands variables like `$PATH`, `$USER`, and custom ones dynamically.

- **Error & Memory Management**  
  Robust error detection and complete memory cleanup on exit.

---

## 🛠️ Technologies Used

- **[C](https://devdocs.io/c/)** — Core programming language.  
- **[Makefile](https://www.gnu.org/software/make/manual/make.html)** — Build automation tool.  
- **[POSIX System Calls](https://man7.org/linux/man-pages/man2/)** — For processes, signals, and file descriptors.  
- **[GNU Readline](https://tiswww.case.edu/php/chet/readline/rltop.html)** — For command-line input handling.

---

## 🚀 How to Build and Run

Clone the repository and compile the project:

```bash
git clone git@github.com:doooriian/Minishell.git
cd Minishell
make
```

Run the program:

```bash
./minishell
```

Example usage inside the shell:

```bash
echo "Hello, Minishell!"
export NAME=Dorian
echo $NAME
ls -la | grep minishell
cat file.txt > output.txt
exit
```

Clean and rebuild:

```bash
make clean
make fclean
make re
```

---

## 🧪 Testing

The project was extensively tested with:
- Basic and complex commands (single, piped, and redirected).  
- Edge cases for syntax errors and invalid inputs.  
- Signal handling during execution and idle mode.  
- Memory management verified using **Valgrind**.  
- Comparison with Bash outputs for consistency.  

---


## 🏅 Results

Here’s my score for the Minishell project:

<p align="center">
  <img src="https://github.com/doooriian/42-Badges/blob/main/badges/MinishellGrade.png" alt="Minishell Grade">
</p>

---

## 📬 Contact

Feel free to reach out or contribute to this project on [GitHub](https://github.com/doooriian)!
