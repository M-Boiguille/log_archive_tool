# Log Archive Tool

Log Archive Tool is a simple Bash script designed to compress log files from a specified directory into a `tar.gz` archive. It addresses common challenges in system administration tasks.

## Features
- Compresses log files into a `tar.gz` archive in a new folder.

Not mandatory:
- Allows specifying an optional output directory.

## Usage
### Syntax
```
./log-archive <log-directory> [output-directory]
```
- **log-directory**: Directory containing the logs to compress.
- **output-directory** (optional): Destination for the archive. Defaults /var/log/.

### Examples
1. Create an archive in the /var/log directory:
   ```bash
   ./log-archive /my/program/logs/
   ```
2. Create an archive in a specified directory:
   ```bash
   ./log-archive /var/log /tmp
   ```

### Output
An archive named `logs_archive_YYYYMMDD_HHMMSS.tar.gz` will be created in the specified output directory.

## Development Environment
- **OS:** Linux (Ubuntu)
- **Language:** Bash
- **Tools:** `tar`, `find`, `rm`, functions, if statement, check file types, ...

### Improvements
- emailing the user updates on the archive
- sending the archive to a remote server or cloud storage.
- delete archived files.

## Conclusion
This project demonstrates a robust and practical solution for compressing log files, with a focus on reliability, clear usage, and error handling.