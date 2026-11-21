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
