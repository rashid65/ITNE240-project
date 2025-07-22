## Linux System Monitoring Tool (Simplified top or htop):

Description: Create a command-line tool that displays real-time system information
such as CPU usage, memory usage, and a list of running processes. This involves
reading data from the /proc filesystem.

Learning Focus: Linux filesystem (/proc), system information retrieval, process
enumeration

```
linux-monitor/
├── internal/
│   ├── cpu/
│   │   ├── cpu.go        # Reads and parses /proc/stat
│   ├── memory/
│   │   ├── memory.go     # Reads and parses /proc/meminfo
│   ├── process/
│   │   ├── process.go    # For listing processes from /proc/[pid]
├── pkg/
│   ├── utils/
│   │   ├── utils.go      # Any helper functions (parsing, formatting)
├── main.go                # Main application loop
├── go.mod                 # Go module definition
├── go.sum                 # Go dependencies checksum
└── README.md               # Documentation on running the tool

```