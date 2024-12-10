# Disk Arm Movement Simulation with FCFS Scheduling

## Features

- **FCFS Disk Scheduling**: Simulates the behavior of the First-Come-First-Served (FCFS) disk scheduling algorithm for track requests.
- **Dynamic Input**: Allows the user to input the initial position of the disk arm, track requests, and other necessary parameters.
- **Movement Tracking**: Tracks the total head movement and the sequence of tracks accessed.
- **Visualization**: Visualizes the disk arm movement with a plot showing the sequence of track accesses and head movements.
- **Metrics**: Calculates and displays the total head movement and seek time.

## Code Explanation

### DiskArm Class

This class simulates the movement of the disk arm in response to track requests. It includes the following attributes and methods:

- **Attributes**:
  - `current_position`: The current position of the disk arm.
  - `total_head_movement`: The total movement of the disk arm across all requests.
  - `seek_time`: The total time taken for the seek operations.
- **Methods**:
  - `move_to(target_track)`: Moves the disk arm to the target track and updates the movement and position.

### process_requests Function

- This function processes the track requests in the order they are received, calculating the total head movement and seek time. It returns the total head movement, seek time, and the sequence of accessed tracks.

### plot_disk_arm_movement Function

- This function generates a plot visualizing the movement of the disk arm across tracks, showing both the order of access and the movement from one track to the next.

### main Function

- The `main` function allows the user to input necessary parameters (such as initial position, track requests, and seek rate) and simulates the disk arm movement, displaying the results and visualizing the movement.

## Running the Program

1. **Dependencies**

   - `matplotlib`: Used for visualizing the disk arm movement.

2. **Running the Program**
   - Run the Python script to simulate the disk arm's movement based on FCFS scheduling.
   - The program will prompt for the following inputs:
     - Initial position of the disk arm.
     - Track requests (list of tracks the disk arm should access).
     - Maximum track number on the disk.
     - Seek rate (time units per track move).
   - After processing the requests, the program will display the total head movement, seek time, and a plot of the disk arm's movement.
