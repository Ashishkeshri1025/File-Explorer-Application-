# File Explorer Application (C++ Console-Based)

The **File Explorer Application** is a console-driven utility developed in **C++**.  
It enables users to perform a comprehensive range of file and directory operations while maintaining a user-friendly command-line interface.  
In addition to basic file handling operations, the application incorporates several advanced features such as activity logging, directory statistics, filtered search, and file comparison utilities.

---

## ✅ Key Features

### **1. Basic File and Directory Operations**
- Listing of directory contents with metadata
- Changing directories, including relative navigation
- Creation of files and directories
- Deletion of files and directories (if empty)
- Copying and moving files between locations
- Displaying file contents with line numbering
- Viewing and modifying file permissions in octal format

### **2. Advanced Functional Modules**
- **Activity Logger:**  
  Records and stores user actions in the log file `file_explorer_activity.log` with timestamps.

- **Directory Statistics Dashboard:**  
  Provides total file count, folder count, cumulative size, and file-type breakdowns.

- **Advanced Search Engine:**  
  Allows searching based on filename pattern, extension filter, and file size range.

- **File Comparison Tool:**  
  Compares two text files line-by-line and reports differences with size analytics.

---

## ✅ Technology and Platform Compatibility

The application utilizes **POSIX APIs**, including:
- `dirent.h`
- `sys/stat.h`
- `unistd.h`

### Platform Support
- ✅ Linux
- ✅ macOS
- ✅ Windows (via **Windows Subsystem for Linux** or MinGW with `dirent` compatibility)

---

## 📦 Build and Execution Guide

### **Prerequisites**
- C++17 compliant compiler (`g++` or `clang++`)
- POSIX-supported environment

### **Compilation Command**
```bash
g++ -std=c++17 -O2 -Wall -Wextra -pedantic main.cpp -o file-explorer
