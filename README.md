# Syscalls used

### 1. Getline()
```cpp
ssize_t getline(char **lineptr, size_t *n, FILE *stream);
```
Description: Reads a line of text from a stream. It can be a file, a pipe or standard input

### 2. Fork()
```cpp
pid_t fork(void);
```
Description: Creates a child process by duplicating the calling process.

### 3. Wait()
```cpp
pid_t wait(int *wstatus);
```
Description: Causes the current processes to wait until of its child process terminates.

### 4. Execve()
```cpp
int execve(const char *pathname, char *const argv[], char *const envp[]);
```
Description: Execute a new programmed referred to by the `pathname` variable. Here, `argv[]` is an array of strings, `envp[]` .......................

### 5. Strtok()
```cpp
char *stork(chat *str, const char *delim);
```
Description: Breaks a string into a sequence of tokens(a sequence of characters seperated by a delim)

### 6. Getenv()
```cpp
char *getenv(const char *name);
```
Description: Searches the environment list to find the environment variable name.

### 7. Stat()
```cpp
int stat(const char *pathname, struct stat *statbuf);
```
Description: Returns the information about the file in the buffer pointed to by the statbuf variable.

### 8. Access()
```cpp
int access(const char *pathname, int mode);
```
Description: Checks whether the file `pathname` can be accessed. Mode:
- F_OK: If file exits
- R_OK: If file exists and grants read permissions
- W_OK: If file exists and grants write permissions
- X_OK: If file exists and grants execute permissions

### 9. Strdup()
```cpp
char *strdup(const char *s);
```
Description: Returns a pointer to a new string which is a duplicate of the string s.

### 10. Isatty()
```cpp
int isatty(int fd);
```
Description: Checks if the file is opened in interactive or non-interactive mode using the file descriptor.


# Misc

#### 1. size_t, ssize_t 
- Count of bytes. Result of `sizeof` operator.
- Included in `<string.h>`, `<sys/types.h>`, ..., etc.

#### 2. pid_t
- Process/User/Group identifier
- `<sys/types.h>`

#### 3. perror()
- print a system error message
- `<stdio.h>`
