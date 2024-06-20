# CPU Scheduler Simulation

This project simulates various CPU scheduling algorithms using C++ and HTML for visualization. It includes implementations of FCFS (First-Come, First-Served), SJF (Shortest Job First), Priority Scheduling, and Round Robin scheduling algorithms.

## Project Structure

- **cpp/**: Contains the C++ source code files.
- **html/**: Contains the HTML and JavaScript files for visualization.
- **input.txt**: Input file containing process arrival times, burst times, and priorities.
- **result.txt**: Output file generated after running the simulation.

## Algorithms Implemented

1. **FCFS (First-Come, First-Served)**:
   - Simulates processes in the order they arrive.

2. **SJF (Shortest Job First)**:
   - Executes the shortest job available first.

3. **Priority Scheduling**:
   - Processes are executed based on priority levels assigned.

4. **Round Robin**:
   - Time-sliced execution where each process gets a small unit of CPU time.

## Running the Simulation

### Prerequisites

- **C++ Compiler**: Ensure you have a C++ compiler installed (e.g., g++ for Linux, MinGW for Windows).

### Steps to Run

1. **Compile C++ Code**:
   - Navigate to the `cd CPU-Scheduler` directory.
   - Compile your C++ source code. For example:
     ```
     g++ CPU-Scheduler.cpp
     ```

2. **Execute the C++ Program**:
   - Run the compiled C++ program to start the simulation and open the HTML visualization:
     ```
     ./a
     ```
   - This will open the default web browser with the simulation results.
  
CPU-Scheduler Report

Project Overview
In this project, I implemented various CPU scheduling algorithms and evaluated them based on parameters such as Finish Time, Turnaround Time, and Wait Time to determine their suitability for a given set of inputs. The parameters considered in the program include the arrival time, burst time, priority of a process, and the timescale. The implemented algorithms are First Come First Serve (FCFS), Shortest Job First (SJF), Priority Scheduling, and Round Robin (RR).

FCFS Algorithm
In the FCFS algorithm, processes are sorted by their arrival time. The process that arrives first is executed first. If two processes have the same arrival time, the one that appears first in the input is executed first. Finish time is calculated during execution, and Turnaround Time and Wait Time are derived from it. A notable issue with FCFS is the potential for process starvation when a large process arrives early.

SJF Algorithm
For the SJF algorithm, processes are first sorted by their arrival time. At each time instant, the shortest job ready for execution is selected and executed. This process continues by selecting the shortest job among available processes. Finish time, Turnaround Time, and Wait Time are calculated similarly to FCFS. This implementation uses a non-preemptive approach and can be improved by implementing a preemptive version for better results.

Priority Scheduling
Processes are sorted by arrival time, and at any given point, the process with the highest priority is executed first. If multiple processes are ready, the one with the highest priority among them is chosen. This implementation considers higher numerical values as higher priority, but user input can be modified to define priority levels. A preemptive version can be implemented for better results.

Round-Robin
In the Round-Robin algorithm, processes are sorted by arrival time and added to a ready queue. Each process in the queue is executed for a time slice, after which the next process in the queue is executed. Any new processes ready for execution are added to the queue. This method reduces response time but increases the finish time for all processes.

Running the Project
- Clone the repository from GitHub and run the provided code with the given input file.

Learning Takeaways
- Gained a comprehensive understanding of various scheduling algorithms, their advantages, and disadvantages.
- Learned the importance of scheduling terms and their impact on selecting the best scheduler.
- Recognized the critical role of schedulers in ensuring efficient execution of tasks in an operating system.
- Enhanced skills in writing clean and efficient C++ code for specific algorithms.
- Learned to integrate front-end and back-end systems to display backend data to users on the front end.

 References

https://www.youtube.com/playlistlist=PLBlnK6fEyqRitWSE_AyyySWfhRgyA-rHk

 https://www.doc-developpement-durable.org/file/Projets-informatiques/cours-&-
manuels-informatiques/Linux/Linux%20Kernel%20Development,
%203rd%20Edition.pdf

 https://www.researchgate.net/publication/
49619229_An_Improved_Round_Robin_Schedduling_Algorithm_for_CPU_Sched
uling

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
