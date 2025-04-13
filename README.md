#  Custom Linux Shell

A fully functional Unix-style shell built from scratch in C++, emulating core features of popular shells like Bash and Zsh. This project demonstrates deep understanding of operating system concepts such as process control, file I/O, signal handling, and job scheduling.

## 🔧 Features

- **Command Parsing** – Supports complex shell commands with arguments
- **Piping (`|`)** – Enables chaining of commands (e.g., `ls | grep txt`)
- **I/O Redirection (`>`, `<`)** – Redirects standard input/output to/from files
- **Job Control** – Supports background execution using `&` and foreground processes
- **Built-in Commands** – Includes shell-native commands like:
  - `cd` – Change directory
  - `exit` – Exit the shell
  - `history` – View command history
- **Tab Completion** – Uses GNU Readline for intelligent auto-completion
- **Environment Variable Expansion** – Expands variables like `$HOME`, `$PATH`
- **Command History** – Persistent command tracking with up/down navigation

## 🛠️ Tech Stack

- **Language**: C++
- **System Calls**: `fork()`, `execvp()`, `pipe()`, `dup2()`, `waitpid()`
- **Libraries**: GNU Readline for input handling and tab completion

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/custom-linux-shell.git
   cd custom-linux-shell
   ```

2. Compile the code:
   ```bash
   g++ shell.cpp -o my_shell -lreadline
   ```

3. Run the shell:
   ```bash
   ./my_shell
   ```

## 📁 Example Usage

```bash
$ ls -l | grep ".cpp" > output.txt &
$ cd /home/user/projects
$ history
```

## 📚 Learnings

- Low-level Unix systems programming
- Process management and job control
- File descriptor manipulation
- Signal handling
- Building extensible parsers for user commands

## 📜 License

This project is open-sourced under the MIT License.

---

Let me know if you want badges (e.g., Build, MIT License, C++ version), contribution guidelines, or a project demo GIF!
