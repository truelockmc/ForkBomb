
# ForkBomb Project

This project includes scripts that demonstrate the concept of a fork bomb, a type of denial-of-service attack that creates numerous processes to overwhelm system resources. The provided scripts are for educational purposes and should only be used in controlled environments.

**WARNING**: Running these scripts can severely impact system performance and stability, potentially causing a system crash or requiring a restart. Use these scripts responsibly and only for educational purposes.

## Scripts

### 1. Batch File Fork Bomb

**Script: `forkbomb1.bat`**

```batch
@echo off
:loop
%0|%0
goto loop
```

**Description**: This batch script continuously runs itself and pipes its output to another instance of itself. This rapid process creation quickly overwhelms the system.

**How to Use**:

1. **Create the Batch File**:
   - Open a text editor (such as Notepad) and paste the above script.
   - Save the file with a `.bat` extension, for example, `forkbomb1.bat`.

2. **Run the Script**:
   - Double-click the `forkbomb1.bat` file to execute it.
   - **Important**: This will rapidly consume system resources. You may need to restart your computer to stop the script.

### 2. Alternative Batch Script Fork Bomb

**Script: `forkbomb2.bat`**

```batch
:(){:|:&};:
```

**Description**: This script creates a fork bomb using a syntax similar to Unix-based fork bombs but in a batch file format. It rapidly creates processes by defining a function and calling it recursively.

**How to Use**:

1. **Create the Batch File**:
   - Open a text editor and paste the above script.
   - Save the file with a `.bat` extension, such as `forkbomb2.bat`.

2. **Run the Script**:
   - Double-click the `forkbomb2.bat` file to execute it.
   - **Important**: This will quickly overwhelm your system. You may need to restart your computer to stop the script.

## Important Notes

- **System Impact**: Both scripts are designed to overwhelm system resources by creating numerous processes. They should only be used in safe, controlled environments.
- **Ethical Considerations**: Do not use these scripts on any system without proper authorization. Unauthorized use can cause significant disruption and is considered malicious activity.
- **Recovery**: If you run these scripts and experience system instability, you may need to restart your computer to recover.

## License

This project is provided for educational purposes under the MIT License. See the [LICENSE](LICENSE) file for more details.
