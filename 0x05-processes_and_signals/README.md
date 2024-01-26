Project Name
PID and Signals README 0x05-processes_and_signals

Overview
This documentation provides insights into how the project manages Process IDs (PIDs) and signals. Understanding these concepts is crucial for efficient process management and communication within the system.

Table of Contents
Introduction
PIDs (Process IDs)
Signals

Introduction
In many computing systems, processes are identified by unique numerical values known as Process IDs (PIDs). Signals, on the other hand, are mechanisms used for inter-process communication and management. This documentation outlines how our project leverages PIDs and signals for effective operation.

PIDs (Process IDs)
Our project assigns and tracks PIDs to manage various processes. PIDs are dynamically assigned during process creation and serve as unique identifiers. The system keeps a record of active PIDs, facilitating efficient communication and control.

Signals
The project utilizes signals to communicate with processes and control their behavior. Common signals include SIGTERM for termination and SIGUSR1 for user-defined actions. Custom signal handlers are implemented to respond appropriately to these signals, ensuring graceful process management.
