# clear_logs.sh

This Bash script scans the project files for log commands and deletes them, while excluding specified directories and files.

## Description

The script is configured to search within the `./src` directory for files ending with `.ts`, `.tsx`, `.js`, or `.jsx`.

There are arrays defined at the top of the script for directories and files to exclude from the operation:

- `EXCLUDE_DIRS`: An array of directory names to exclude. The script will not perform operations on files within these directories.
- `EXCLUDE_FILES`: An array of file names to exclude. The script will not perform operations on these files.

The script loops through each file found, checks if the file's directory or the file itself is in the excluded list, and if not, performs operations on the file.

## Usage

To run the script, navigate to the directory containing the script and use the following command:

```bash
./clear_logs.sh
```

Make sure the script has execute permissions. If not, you can add them with:
```bash
chmod +x clear_logs.sh
```

Customization
You can customize the script by modifying the DIR, EXCLUDE_DIRS, and EXCLUDE_FILES variables at the top of the script to fit your needs.

