# 📄 get_next_line - 42 School Project

**get_next_line (GNL)** is a C project from **42 School** where you implement a function to **read a file line by line**, returning one line per call.  
The project teaches memory management, static variables, file descriptors, and buffer handling in C.

---

## 🎯 Project Goals

- Implement a function `get_next_line` with the prototype:  
```c
int get_next_line(int fd, char **line);

The bonus part requires supporting multiple file descriptors at the same time, meaning that reading from fd1 and fd2 alternately should work independently.
