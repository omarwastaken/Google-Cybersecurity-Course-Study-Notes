# Linux and SQL
---
#### In this course, you will:

- Describe the main functions of an operating system
- Explain the relationship between operating systems, applications, and hardware
- Compare a graphical user interface to a command line interface
- Navigate the file system using Linux commands via the Bash shell
- Use SQL to retrieve information from a database

#### Skill sets:

- Interacting with both a graphical user interface (GUI) and command line interface (CLI)
- Querying a database with SQL
- Filtering on a particular word with the Linux command line
- Authenticating and authorizing users with the Linux command line

---
## Comparing Operating Systems for Security Professionals

This reading explores popular operating systems and the security considerations associated with them.

### Common Operating Systems

Here's a list of operating systems relevant to the security field:

- Windows
- macOS®
- Linux
- ChromeOS
- Android
- iOS

### Windows and macOS

- Introduced in 1984 and 1985 respectively, both Windows and macOS are widely used on personal and enterprise computers.
- Windows is closed-source, meaning its source code isn't publicly available.
- macOS is partially open-source, with some components like the kernel being open.

### Linux

- Released in 1991, Linux is a fully open-source operating system. This allows collaboration among developers in the Linux community.
- Due to its open-source nature, Linux plays a significant role in the security industry. Specific distributions cater to security professionals (covered later in the course).

### ChromeOS

- Launched in 2011, ChromeOS is partially open-source, derived from the fully open-source Chromium OS.
- ChromeOS is commonly used in educational settings.

### Android and iOS

- Introduced in 2007 and 2008 respectively, Android (open-source) and iOS (partially open-source) are mobile operating systems used on devices like phones, tablets, and watches.

### Operating Systems and Vulnerabilities

- All operating systems are susceptible to security vulnerabilities. Keeping the system and its components updated is crucial for maintaining security.

### Legacy Operating Systems

- Legacy operating systems are outdated systems still in use.
- Organizations might rely on legacy systems due to software incompatibility with newer versions. This is common in industries using equipment with embedded software.
- Legacy operating systems become vulnerable due to lack of support and updates, making them susceptible to new threats.

### Other Vulnerabilities

- Even updated operating systems can have vulnerabilities. Here are some resources for staying informed:
    - Microsoft Security Response Center (MSRC): Lists known vulnerabilities in Microsoft products and services.
    - Apple Security Updates: Provides security updates and information for Apple® products (macOS, iOS, etc.).
    - Common Vulnerabilities and Exposures (CVE) Report for Ubuntu: Lists known vulnerabilities affecting the Linux distribution, Ubuntu.
    - Google Cloud Security Bulletin: Lists known vulnerabilities affecting Google Cloud products and services.

### Key Takeaways

- Security analysts should be familiar with common operating systems (Windows, macOS, Linux, ChromeOS, Android, iOS) and their vulnerabilities.
- Legacy operating systems, though outdated, are still in use and pose significant security risks due to lack of updates.

---
## How Operating Systems Work

This reading explains the role of operating systems (OS) in managing computer tasks and the importance of understanding this process for security analysts.

### Booting the Operating System

- Booting refers to the process of starting a computer.
- Pressing the power button triggers the boot process, activating the BIOS (or UEFI in newer systems).
- The BIOS/UEFI contains instructions for loading the bootloader, a program responsible for starting the operating system.
- Understanding the booting process is crucial for security analysts because vulnerabilities can exist here (e.g., malware infection in BIOS). Antivirus software might not scan the BIOS, making it a potential security risk.

### User Interaction and Application Execution

- Users interact with computers through applications (programs designed for specific tasks).
- When a user opens an application, it sends a request to the operating system.
- The operating system interprets the request and directs it to the appropriate hardware component.

**Hardware Recap**

- Hardware refers to the physical components of the computer.
- Hardware components communicate with the operating system as well, sending information back and forth.

### Example: Using the Calculator

1. The user clicks on the calculator application.
2. The calculator application communicates with the operating system.
3. The operating system sends the calculation task to the CPU (central processing unit).
4. The CPU performs the calculation and sends the answer back to the operating system.
5. The operating system displays the answer in the calculator application window.

### Significance for Security Analysts

Understanding this interaction flow between user, application, operating system, and hardware is vital for security analysts. It allows them to trace back the steps involved in a security event and pinpoint where the breach might have occurred.

**Analogy:** Similar to how a mechanic needs a deeper understanding of a car's inner workings compared to a casual driver, security analysts need a strong grasp of operating system functions to effectively analyse security issues.

## Understanding Operating Systems: A Behind-the-Scenes Look

This reading dives deeper into the inner workings of operating systems (OS) and how they facilitate user interaction with computers.

### Booting Up: The Initiation Process

- Booting refers to starting a computer.
- BIOS (Basic Input/Output System) or UEFI (Unified Extensible Firmware Interface) chips are activated during boot.
    - BIOS: Found in older systems, contains instructions for loading the computer.
    - UEFI: Modern replacement for BIOS, offers enhanced security features.
- Both BIOS/UEFI perform the same booting function.
- These chips provide instructions like verifying hardware health before activating the bootloader, a program that launches the operating system.

### Completing a Task: A Four-Step Journey

1. **User:** The initiator, wanting to accomplish a task on the computer (e.g., reading this document).
2. **Application:** The software program used to complete the task (e.g., calculator for calculations, word processor for reports).
3. **Operating System:** The intermediary, receiving the user's request from the application, interpreting it, and directing it to the relevant hardware.
4. **Hardware:** Where the actual processing occurs (e.g., CPU performing calculations, hard drive storing files). Hardware then sends the results back to the application.

**Analogy: Car vs. Computer**

Similar to a car (pressing the gas pedal for movement without understanding the engine's inner workings), users interact with computers without directly observing the OS at work.

**Analogy: Restaurant Order**

Using an OS is like ordering at a restaurant:

- User (customer): Places an order (requests an action through an application).
- Application (waiter): Takes the order (receives the user's request).
- OS (kitchen): Processes the order (interprets the request and directs it to the hardware).
- Hardware (cooks): Completes the order (performs the task using hardware components).
- Application (waiter): Delivers the completed order (shows the results to the user).
- User (customer): Receives the completed order (experiences the results).

**Example: Downloading a File**

This example demonstrates OS, application, and hardware collaboration:

1. User initiates a download from a web browser.
2. Web browser communicates the download request to the OS.
3. OS directs the request to the appropriate hardware.
4. Hardware downloads the file and informs the OS.
5. OS relays the download completion status to the web browser.
6. Web browser notifies the user that the download is finished.

### Key Takeaway

The operating system, although working behind the scenes, plays a critical role in enabling users to interact with computers and complete tasks. It acts as a bridge connecting applications and hardware components to execute user requests.

## Resource Management by the Operating System

This reading explores the role of the operating system (OS) in managing computer resources efficiently.

### Balancing Resource Allocation

- Similar to how humans require varying energy levels for different tasks (running vs. watching TV), the OS ensures sufficient resources are available for specific computer tasks (antivirus scan vs. calculator).

### The OS as a Conductor

- The OS acts like an orchestra conductor, directing the flow of resources.
- Limited computer resources (CPU, memory, storage, bandwidth) are constantly in demand by various programs, tasks, and processes.
- The OS allocates and deallocates resources as needed, ensuring efficient system function.

**Behind-the-Scenes Management**

- Most of this resource management occurs transparently to the user.

### Task Manager and Resource Monitoring

- The task manager provides a view of running tasks, along with their CPU and memory usage.

### Importance for Security Analysts

- Understanding resource usage helps analysts:
    - Respond to security incidents.
    - Troubleshoot applications.
    - Identify malicious activity (e.g., malware hogging resources and causing slowdowns).

**Overall Takeaway**

A fundamental understanding of OS resource management strengthens the foundation for security skills learned later in the program.

## Virtualization Technology for Security Professionals

This reading explores virtual machines (VMs) and virtualization concepts, highlighting their benefits and importance in the security field.

### What are Virtual Machines (VMs)?

- A VM is a software emulation of a physical computer system.
- It functions like a physical computer but lacks a physical presence, relying on software-defined resources.
- VMs have virtual versions of CPU, storage, and other hardware components.

### Running Multiple VMs on a Single Machine

- Virtualization software allows running multiple VMs on a single physical computer's hardware resources.
- These resources are shared and allocated among the physical machine and VMs (e.g., RAM divided between VMs and the physical machine).
- Each VM can have its own operating system and function independently like a typical computer.

### Benefits of Virtual Machines for Security

- **Security:** VMs provide isolated environments (sandboxes) on the host machine.
    - Guest VMs are isolated from the host and other guest VMs, enhancing security.
    - This isolation allows for safer malware analysis within a VM if it becomes infected.
    - Security professionals can intentionally introduce malware into a VM for controlled examination.
- **Efficiency:** VMs offer a convenient and efficient way to perform security tasks.
    - Users can open and switch between multiple VMs for streamlined security testing and application exploration.
    - The efficiency is analogous to a city bus transporting many people compared to everyone using individual cars. Similarly, VMs optimize resource usage by running multiple VMs on a single physical machine.

**Note:** While VMs are valuable for testing malware and isolating risky software, there's still a possibility of malicious programs escaping the virtual environment and compromising the host machine. Therefore, complete trust in virtualized systems is not advised.

### Managing Virtual Machines with Hypervisors

- Hypervisors are software programs that manage VMs and bridge the gap between virtual and physical hardware.
- They allocate shared resources from the physical host machine to VMs.
- **Kernel-based Virtual Machine (KVM):** An important open-source hypervisor supported by major Linux distributions.
    - Built into the Linux kernel, KVM allows creating VMs on any Linux machine without additional software.

### Other Forms of Virtualization

- Beyond VMs, virtualization encompasses other technologies that don't necessarily involve operating systems.
    - Virtual servers: Creating multiple virtual servers from a single physical server.
    - Virtual networks: Creating virtual networks to optimize hardware utilization within a physical network.

### Key Takeaways

- VMs are essential in the security field, allowing creation and management of isolated computer environments.
- Understanding VM benefits (security isolation, efficiency) is crucial for security professionals.
- While VMs enhance security, potential risks of malware escape necessitate caution.

---
## User Interfaces: Communicating with Operating Systems

This reading explores how users interact with computers through user interfaces (UIs). It highlights two main UI types: graphical user interfaces (GUIs) and command-line interfaces (CLIs).

### User Interfaces: The Bridge Between User and OS

- A user interface (UI) is a program that facilitates user interaction with the operating system (OS).
- It allows users to control the OS and execute tasks on the computer hardware.

### Graphical User Interface (GUI)

- A GUI is an icon-based user interface that provides a visual way to interact with the computer.
- Most modern operating systems offer a GUI environment.
- Common GUI components include:
    - Start menu: Provides access to programs grouped by category.
    - Taskbar: Displays running applications and allows launching new ones.
    - Desktop: Houses icons and shortcuts for easy access to programs and files.
- Users can interact with a GUI by clicking icons, searching for programs, or using menus.

### Command-Line Interface (CLI)

- In contrast to the GUI, a CLI is a text-based user interface that relies on typed commands to interact with the computer.
- CLIs require users to enter specific commands to execute tasks and launch programs.
- The CLI offers a different experience compared to the GUI:
    - No icons or graphics - resembles lines of code.
    - More flexible and powerful than a GUI.

**Analogy: GUI vs. CLI**

- Using a GUI is similar to ordering food at a restaurant:
    - Limited options based on the menu.
    - Tasks must be completed one at a time.
- Using a CLI is like creating a custom meal from scratch:
    - Offers greater control and customization.
    - Allows for performing multiple tasks simultaneously (e.g., moving multiple files at once).

### Importance for Security Analysts

- Security professionals often use CLIs for tasks like:
    - Analyzing log files.
    - Authenticating and authorizing users.
- Later in the program, you'll gain hands-on experience using the command line in Linux, a valuable skill for security analysts.

**Key Takeaways**

- GUIs provide a user-friendly graphical interface for interacting with the OS.
- CLIs offer a more powerful and flexible way to interact with the computer using text commands.
- Understanding both GUIs and CLIs is essential for security professionals due to their use in various security tasks.

## Command Line vs. Graphical User Interface: A Security Analyst's Perspective

This reading dives deeper into the comparison between graphical user interfaces (GUIs) and command-line interfaces (CLIs), emphasizing their relevance in cybersecurity.

### GUI vs. CLI: A Review

- **GUI (Graphical User Interface):** Uses icons and graphics for user interaction.
    - Examples: Icons on desktops, menus, taskbars.
- **CLI (Command-Line Interface):** Text-based interface requiring typed commands for interaction.
    - Resembles lines of code.

### Key Differences in Appearance and Function

- **Display:** GUIs are visually rich with icons and graphics, while CLIs are purely text-based.
- **Functionality:** GUIs typically handle one request at a time, while CLIs can handle multiple requests simultaneously.

### Advantages of CLI for Security Analysts

- **Efficiency:** For experienced users, CLIs can be faster due to accepting multiple commands at once.
    - Example: Creating multiple files in the system is quicker with a CLI compared to a repetitive GUI process.
- **History File:** Linux CLIs maintain a history of all executed commands, beneficial for security analysts in:
    - **Playbook Verification:** Reviewing a series of commands used while following a security incident response playbook.
    - **Intrusion Detection:** Potentially tracing an attacker's actions through the command history.

### Key Takeaways

Security professionals should be comfortable using both GUIs and CLIs due to their distinct functionalities.

- GUIs offer a user-friendly graphical environment for general interaction.
- CLIs provide power and efficiency for security tasks, particularly when handling multiple commands or reviewing historical actions.

Understanding both interface types equips security analysts with the flexibility to choose the most appropriate tool for the situation.

---
## Glossary terms from module 1


**Application:** A program that performs a specific task

**Basic Input/Output System (BIOS):** A microchip that contains loading instructions for the computer and is prevalent in older systems 

**Bootloader:** A software program that boots the operating system

**Command-line interface (CLI):** A text-based user interface that uses commands to interact with the computer

**Graphical user interface (GUI):** A user interface that uses icons on the screen to manage different tasks on the computer

**Hardware:** The physical components of a computer

**Legacy operating system:** An operating system that is outdated but still being used

**Operating system (OS)**: The interface between computer hardware and the user

**Random Access Memory (RAM):** A hardware component used for short-term memory

**Unified Extensible Firmware Interface (UEFI):** A microchip that contains loading instructions for the computer and replaces BIOS on more modern systems

**User interface:** A program that allows the user to control the functions of the operating system

**Virtual machine (VM)**: A virtual version of a physical computer