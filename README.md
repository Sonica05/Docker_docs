# Docker_docs

### 🔹 **What is a Container?**

A **container** is a standard unit of software that **packages up an application** along with **everything it needs to run** — like libraries, dependencies, and configuration files.

> ✅ This makes it possible to run the application **consistently across different environments**, whether it's a developer’s laptop, a testing server, or a production cloud.

#### 🔸 Simplified:

> A **container = Application + App Libraries + Minimum System Dependencies**

Think of it like a **portable, self-contained box** that holds everything your application needs to run — so it works **the same way** everywhere.

---

### 🐳 **What is a Docker Container Image?**

A **Docker container image** is a **lightweight, standalone, executable package** that contains:

* Application code
* Runtime (e.g., Node.js, Python, Java)
* System tools and libraries
* Required settings

When this image runs, it becomes a **Docker container** — an isolated process on your machine.

---

### 🔄 **Containers vs Virtual Machines (VMs)**

| Feature          | **Containers**               | **Virtual Machines (VMs)** |
| ---------------- | ---------------------------- | -------------------------- |
| **OS**           | Share the **host OS kernel** | Each VM has its **own OS** |
| **Size**         | Lightweight                  | Heavy                      |
| **Startup Time** | Seconds                      | Minutes                    |
| **Performance**  | Fast                         | Slower                     |
| **Portability**  | Highly portable              | Less portable              |
| **Isolation**    | Process-level                | Full OS-level isolation    |
| **Resource Use** | Efficient                    | Resource-heavy             |

> 🔍 Example: Running 10 containers is much faster and uses fewer resources than running 10 VMs.

---

### ❓ **Why Are Containers Lightweight?**

Containers are lightweight because:

* They **share the host OS kernel**, so no need to include a full operating system.
* They **only contain the necessary files**: app code + libraries + configs.
* They start as fast as a process, unlike VMs which boot up entire OS instances.

 ### Files and Folders in containers base images
 
   * /bin: contains binary executable files, such as the ls, cp, and ps commands.

   * /sbin: contains system binary executable files, such as the init and shutdown commands.

   * /etc: contains configuration files for various system services.

   * /lib: contains library files that are used by the binary executables.

   * /usr: contains user-related files and utilities, such as applications, libraries, and documentation.

   * /var: contains variable data, such as log files, spool files, and temporary files.

   * /root: is the home directory of the root user.

### Files and Folders that containers use from host operating system

