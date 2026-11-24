# Linux Commands and Troubleshooting

This document records the Linux commands and troubleshooting concepts I have learned while preparing for a Forward-Deployed Engineer (FDE) / Software Implementation role.

The focus is on practical Linux usage for application support, log analysis, troubleshooting, and warehouse automation environments.

---

## 1. Navigating the Filesystem

### `pwd`

**What it does:**

`pwd` stands for "print working directory." It shows the directory I am currently working in.

**Example:**

```bash
pwd
```

**What I learned:**

I can use `pwd` to confirm exactly where I am before working with files or directories.

**FDE relevance:**

When troubleshooting an application or working with deployment files, knowing the current directory helps avoid running commands against the wrong location.

---

### `ls`

**What it does:**

`ls` lists the files and directories in the current location.

**Example:**

```bash
ls
```

**What I learned:**

I can use `ls` to see what files and folders are available in my current directory.

**FDE relevance:**

Useful when locating application files, scripts, configuration files, logs, or other deployment-related files.

---

### `cd`

**What it does:**

`cd` stands for "change directory." It moves me from one directory to another.

**Example:**

```bash
cd 01-linux
```

**What I learned:**

I used `cd` to move from the main GitHub repository directory into the `01-linux` directory.

**FDE relevance:**

FDE troubleshooting often requires moving between application, configuration, log, and script directories.

---

### `mkdir`

**What it does:**

`mkdir` creates a new directory.

**Example:**

```bash
mkdir 01-linux
```

**What I learned:**

I used `mkdir` to create the `01-linux` directory for organizing my Linux learning documentation.

**FDE relevance:**

Directories can be used to organize scripts, logs, configuration files, test data, and troubleshooting artifacts.

## 2. Working with Files and Directories

### `touch`

**What it does:**

`touch` creates an empty file if the file does not already exist. If the file already exists, it updates the file's timestamp without removing its contents.

**Example:**

```bash
touch test.log
```

**What I learned:**

I used `touch` to create files that can later be used for logs, test data, scripts, or other troubleshooting activities.

**FDE relevance:**

FDE work often involves creating log files, test files, scripts, and diagnostic artifacts while troubleshooting or validating an environment.

---

### `cat`

**What it does:**

`cat` displays the contents of a file in the terminal.

**Example:**

```bash
cat warehouse.log
```

**What I learned:**

`cat` is useful for quickly viewing the contents of a log or text file. It displays the file contents; it does not list files inside a directory.

**FDE relevance:**

During troubleshooting, `cat` can be used to quickly inspect configuration files, logs, test data, and diagnostic output.

---

### `echo`

**What it does:**

`echo` displays text in the terminal and can also be used with redirection to write text into a file.

**Example:**

```bash
echo "Health check started"
```

**What I learned:**

I learned that `echo` can be combined with `>` and `>>` to write information into files.

**FDE relevance:**

`echo` can be useful in Bash scripts for displaying status messages and recording diagnostic information.

---

### `>` — Overwrite / Redirect

**What it does:**

`>` redirects output into a file. If the file already contains information, its existing contents are overwritten.

**Example:**

```bash
echo "System started" > system.log
```

**What I learned:**

A single `>` replaces the existing contents of the target file.

**FDE relevance:**

Output redirection can be useful when creating a fresh diagnostic or test output file.

---

### `>>` — Append / Redirect

**What it does:**

`>>` redirects output into a file while preserving the existing contents and adding the new information at the end.

**Example:**

```bash
echo "Health check completed" >> system.log
```

**What I learned:**

A double `>>` appends information instead of overwriting the existing file.

**FDE relevance:**

Appending is particularly useful for maintaining diagnostic or operational logs where previous entries must be preserved.
