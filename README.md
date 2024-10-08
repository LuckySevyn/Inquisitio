
```
  
                  ██╗███╗   ██╗ ██████╗ ██╗   ██╗██╗███████╗██╗████████╗██╗ ██████╗ 
                  ██║████╗  ██║██╔═══██╗██║   ██║██║██╔════╝██║╚══██╔══╝██║██╔═══██╗
                  ██║██╔██╗ ██║██║   ██║██║   ██║██║███████╗██║   ██║   ██║██║   ██║
                  ██║██║╚██╗██║██║▄▄ ██║██║   ██║██║╚════██║██║   ██║   ██║██║   ██║
                  ██║██║ ╚████║╚██████╔╝╚██████╔╝██║███████║██║   ██║   ██║╚██████╔╝
                  ╚═╝╚═╝  ╚═══╝ ╚══▀▀═╝  ╚═════╝ ╚═╝╚══════╝╚═╝   ╚═╝   ╚═╝ ╚═════╝  by LuckSevyn
```
## Overview
**Inquisitio** is a tool that I designed to gather comprehensive system information from a Windows machine. The tool collects details such as OS version, user accounts, network configuration, firewall settings, running services, scheduled tasks, and much more. It outputs all collected information into a neatly formatted log file named `Inquisitio.txt`, which is saved in the same directory where the tool is executed.

## Features
- Displays a custom banner before running the system commands.
- Collects detailed system information:
  - Operating system version and hostname
  - Current user information
  - User accounts on the system
  - IP configuration details
  - Routing table, ARP cache, and active network connections
  - Group policy results
  - Firewall state and configuration
  - Scheduled tasks and running services
  - Drivers installed on the system
  - Registry information regarding AlwaysInstallElevated policy
  - Searches for sensitive files (e.g., files containing "pass", "cred", or `.config` files)
- Generates a log file (`Inquisitio.txt`) summarizing all information in a readable format.
- Simple to use with no prerequisites other than running the tool on a Windows system.

## How to Use

1. **Download the Tool:**
   Save the tool (`Inquisitio.bat`) or (`Inquisitio.exe`) to any directory on your Windows machine.

2. **Run the Tool:**
   - Open a Command Prompt with **Administrator privileges** (right-click on the Command Prompt icon and select *Run as administrator*).
   - Navigate to the directory where `Inquisitio.bat` or `Inquisitio.exe` is located.
   - Type one of the following commands (depending on which one you would like to use) and hit **Enter**:
     ```cmd
     Inquisitio.bat
     ```
     ```cmd
     Inquisitio.exe
     ```

3. **Wait for Execution:**
   - The tool will open and display a banner and a message: "Please wait for the results...".
   - The system commands will execute, and the results will be compiled and saved to a log file.
   - If you encounter any errors like a registry key or value missing, it will display "ERROR" and "File Not Found" simply saying it is not present on the system.

4. **View the Log File:**
   - Once the tool completes, a file named `Inquisitio.txt` will be created in the same directory as the tool.
   - Open the log file with any text editor (e.g., Notepad) to view the system information collected.

5. **Completion:**
   - After the execution, the tool will notify you that the report was generated and pause until you press any key to exit.

## Tool Output

The generated log file (`Inquisitio.txt`) contains the following sections:
- **Operating System Information**: OS name and version.
- **Hostname**: The system’s hostname.
- **Current User**: The user running the script.
- **User Accounts**: All user accounts on the system.
- **IP Configuration**: Detailed network settings.
- **Routing Table**: Network routes configured on the system.
- **ARP Cache**: A list of IP-to-MAC address mappings.
- **Network Connections**: Active network connections.
- **Group Policy Result**: Applied group policies on the system.
- **Firewall State and Configuration**: Firewall status and rules.
- **Scheduled Tasks**: Tasks configured to run on the system.
- **Running Tasks and Services**: Currently running tasks and their associated services.
- **Running Services**: List of services currently running on the system.
- **Drivers List**: All device drivers installed.
- **Registry Information**: Checks for the AlwaysInstallElevated policy in the Windows registry.
- **Sensitive File Search**: Searches for files with keywords such as "pass", "cred", or with the `.config` extension.

## License
This tool is provided as-is and is meant for educational and administrative purposes. Use responsibly.
