# Infernal Patch Generator
The Infernal Launcher Patch Tool is designed to help users easily generate patch manifests for software updates. It allows users to select files or directories, compress them into .gz format, and generate a list of compressed files for easy patch distribution. The tool is especially useful in software development environments where frequent patches or updates are necessary.

# Features
- File and Folder Management:
Drag-and-drop interface to add files or directories.
Recursive folder inclusion: All files and subdirectories are added when a directory is selected.
File exclusion: Automatically excludes index.php and index.html files, which are not required in patches.
Clear option to remove all files and directories.
Patch Manifest Generation:

- Generates a compressed file (list.txt.gz) that contains a manifest of files with details like last modification date and file size.
Compresses all added files into .gz format for efficient transfer.
Ensures that files in subdirectories are compressed while maintaining the directory structure.
Handles large sets of files efficiently, with a progress bar indicating the current task and progress percentage.

- Automatic Version Incrementing:
The tool reads the version from the settings.conf file, increments it automatically, and updates it back into the file.
The version is included in the generated patch manifest, helping track patch updates.

- Configuration File Handling:
settings.conf file includes configurable OutputPath, PatchVersion and Header.
If the configuration file doesn't exist, the tool creates it with default values.
Reads the output path and patch version from the configuration file for accurate manifest generation.

- Progress Bar & Logging:
Progress bar and status messages update in real time while files are being processed.

- File Size Formatting:
Displays file sizes in a user-friendly format (KB, MB, GB) instead of bytes.
Easily readable file sizes in the list view for user convenience.

- User Interface:
Simple, intuitive UI with a Windows Forms interface.
Settings menu to configure output directory and patch version.
Multiple actions such as adding files, folders, removing files, and generating patches from the menu.

# Configuration
To set the settings for the tool, simply click on Menu > Settings.
You will see three inputs (Header, Output, Patch Version) these are to set the output directory, header name for list.txt and auto increment of patch version.

# Usage
No special permissions are required to run the tool, but administrative privileges may be necessary if the user wants to write to protected directories.

# System Requirements for Running the Tool:
- Operating System:
Windows 10 or higher (64-bit recommended).
.NET Runtime:

- The tool is built using .NET 6.0. Therefore, the user must have the .NET 6.0 Runtime installed on their machine.
