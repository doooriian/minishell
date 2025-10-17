<br />
<p align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8d/42_Logo.svg/1200px-42_Logo.svg.png" alt="42 Logo" width="250" height="250">
  </a>

  <h1 align="center">Minishell</h1>

  <p align="center">
    A simplified UNIX shell implementation from 42 School
    <br /><br />
    <img src="https://github.com/doooriian/42-Badges/blob/main/badges/minishellm.png" alt="Minishell Badge" width="150">
  </p>
</p>

<p align="center">
  <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/doooriian/Minishell?color=1A237E" />
  <img alt="Code language count" src="https://img.shields.io/github/languages/count/doooriian/Minishell?color=00BCD4" />
  <img alt="GitHub top language" src="https://img.shields.io/github/languages/top/doooriian/Minishell?color=7B1FA2" />
  <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/doooriian/Minishell?color=D32F2F" />
</p>

---

## ✨ Overview

**Minishell** is an individual project at 42 School that recreates a simplified version of a UNIX shell.  
This project challenges your understanding of **process creation**, **pipes**, **redirections**, **signals**, and **environment management** — all core concepts of systems programming in C.

The goal? Build a fully functional shell that mimics Bash-like behavior while adhering to 42’s strict coding standards.

---

## 📑 Key Features

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


## ✅ Results

Here’s my score for the Minishell project:

<p align="center">
  <img src="https://github.com/doooriian/42-Badges/blob/main/badges/100Grade.png" alt="Minishell Grade">
</p>

---

## 📬 Contact

Feel free to reach out or contribute to this project on [GitHub](https://github.com/doooriian)!
