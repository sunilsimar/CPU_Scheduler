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

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
