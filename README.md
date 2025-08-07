# Dash

This is a simple shell program written in C. It provides a basic command-line interface where users can enter commands, and the shell will execute them.

## Features

*   **Command Execution:** Executes commands with their arguments.
*   **PATH Handling:** Searches for executables in the system's PATH environment variable.
*   **Basic Prompt:** Displays a simple prompt `Dashed$ ` to indicate that it's ready to receive a command.

## Getting Started

### Prerequisites

*   A C compiler (e.g., `gcc`)
*   `cmake`

### Building

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your_username/Dash.git
    cd Dash
    ```
2.  **Create a build directory:**
    ```bash
    mkdir build
    cd build
    ```
3.  **Configure the project with CMake:**
    ```bash
    cmake ..
    ```
4.  **Compile the project:**
    ```bash
    make
    ```

## Usage

After building the project, you can run the shell from the project's root directory:

```bash
./build/Dash
```

You will be greeted with the `Dashed$ ` prompt. You can then type commands and press Enter to execute them.

```
Dashed$ /bin/ls
CMakeLists.txt  README.md  build  file_loc.c  main.c  main.h
Dashed$
```

### Known Limitations

*   Does not handle built-in commands (e.g., `cd`, `exit`).
*   No support for piping, redirection, or other advanced shell features.
*   Basic error handling.

## Project Structure

*   `main.c`: The main entry point of the shell, containing the read-execute loop.
*   `main.h`: Header file with function prototypes and included libraries.
*   `file_loc.c`: Contains functions for locating executables in the `PATH`.
*   `CMakeLists.txt`: The build configuration file for `cmake`.
*   `README.md`: This file.
