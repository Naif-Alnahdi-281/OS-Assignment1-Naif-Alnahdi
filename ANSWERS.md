Question 1: Thread vs Process

Process is a full program running in the system and it has its own memory. Thread is a smaller part inside process and share memory with other threads. Creating process needs more resources and time, but thread is lighter and faster. In this assignment we used threads because all processes run inside one program and share ready queue and data. Threads make the CPU scheduling simulation easier and faster.

Question 2: Ready Queue Behavior

In Round Robin scheduling, if process does not finish in time quantum, it leaves CPU and goes back to ready queue again. CPU runs other processes first before this process runs again. The process keeps taking turns until remaining time becomes zero. This makes scheduling fair because all processes get chance to use CPU.

Example from my output:

P2 executing quantum
Remaining time: 1500ms
P2 yields CPU for context switch
P2 added to ready queue

Explanation of example:

In this example P2 did not finish after first quantum, so it returned to ready queue to wait for next turn. Other processes run before it. After that P2 runs again until it finishes. This shows how Round Robin shares CPU between processes fairly.

Question 3: Thread States
New: P1 is in New state when thread is created using new Thread.
Runnable: P1 becomes Runnable when start() method is called.
Running: P1 is Running when CPU executes run() method.
Waiting: P1 is Waiting when sleep() is used to simulate burst time.
Terminated: P1 becomes Terminated when remaining time becomes zero and process finishes execution.
Question 4: Real-World Applications
Example 1: Web Server

Description:
Web server handles many user requests at the same time.

Why Round-Robin works well here:
Round Robin gives each request small CPU time so system stays fast and fair. No request takes CPU for long time alone.

Example 2: Operating System Programs

Description:
Operating system runs many programs together like browser, music player, and background apps.

Why Round-Robin works well here:
Round Robin gives each program a turn to use CPU so system stays smooth and responsive.

Summary

Key concepts I understood through these questions:

I learned how Round Robin scheduling works and how processes take turns using CPU. I understood the difference between thread and process. This assignment helped me understand basic idea of CPU scheduling.
