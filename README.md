# Process Monitoring GUI

## Overview

The Process Monitoring GUI is a Python-based application that provides a user-friendly interface to monitor and manage system processes. It allows users to view running processes, track CPU and memory usage, filter processes via a search bar, and terminate selected processes. Additionally, it provides system performance advice and an option to restart the application with administrator privileges when needed.

## Features

- **View Running Processes:** Displays a list of currently running processes along with CPU usage, memory usage, network usage, and disk usage.
- **Search Functionality:** Allows users to filter processes by name using a search bar.
- **Terminate Processes:** Enables users to kill a selected process (requires admin privileges for system processes).
- **Performance Advice:** Provides recommendations based on high CPU, memory, or disk usage.
- **Run as Administrator:** If a process requires admin privileges to be terminated, the application prompts the user to restart as an administrator.

## Requirements

- Python 3.x
- Required Python Libraries:
  - `psutil` (for process monitoring)
  - `tkinter` (for GUI)
  - `ctypes` (for requesting admin privileges)
  - `sys` (for script relaunching)

## Installation

1. Clone the repository or download the script.
   ```sh
   git clone https://github.com/your-repo/process-monitoring-gui.git
   cd process-monitoring-gui
   ```
2. Install dependencies using pip:
   ```sh
   pip install psutil
   ```
3. Run the script:
   ```sh
   python process_monitor_gui.py
   ```

## Usage

- Launch the application.
- Use the search bar to filter specific processes.
- Select a process from the list and click "Kill Selected Process" to terminate it.
- If admin rights are needed, the application will prompt for permission and restart with elevated privileges.
- Click "Get Advice" to receive performance recommendations.

## Notes

- Some system processes require administrator privileges to be terminated.
- If admin rights are granted, the script will restart itself with elevated permissions.
- Ensure Python and required dependencies are installed before running the script.

## License

This project is open-source and available under the MIT License.

## Author

Developed by Kishlay Kumar
