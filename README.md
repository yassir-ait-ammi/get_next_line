# 📄 get_next_line - 42 School Project

**get_next_line (GNL)** is a C project from **42 School** where you implement a function to **read a file line by line**, returning one line per call.  
The project teaches memory management, static variables, file descriptors, and buffer handling in C.

---

## 🎯 Project Goals

- Implement a function `get_next_line` with the prototype:  
```c
int get_next_line(int fd, char **line);
Read a line from a file descriptor fd and store it in *line.

Handle multiple file descriptors simultaneously (bonus part).

Manage memory properly without leaks.

📚 Function Behavior
Returns 1 if a line has been read.

Returns 0 if the end of the file has been reached.

Returns -1 in case of an error (invalid fd, memory allocation failure).

Requirements:
Use a BUFFER_SIZE macro to define the size of the read buffer.

Handle files of any size, including very large files.

Lines are terminated by \n (newline). The newline should not be included in the returned string.

🚀 Bonus Part
The bonus part requires supporting multiple file descriptors at the same time, meaning that reading from fd1 and fd2 alternately should work independently.

📁 Project Structure
bash
Copy code
get_next_line/

├── includes/

│   └── get_next_line.h   # Header file with prototypes

├── srcs/

│   ├── get_next_line.c   # Main function

│   ├── get_next_line_utils.c  # Helper functions

│   └── bonus/            # Bonus part helpers

├── Makefile              # Build library

└── README.md

⚙️ Compilation
To compile the library:

bash
Copy code
make
This will generate:

Copy code
libftgnl.a
To clean object files:

bash
Copy code
make clean
To remove object files and the library:

bash
Copy code
make fclean
To rebuild the library:

bash
Copy code
make re
