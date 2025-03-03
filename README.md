# rm-trailing-whitespaces

## Description

This script removes trailing whitespaces from files. It can process individual files, entire directories, or prompt the user for confirmation before modifying all files in the current directory and subdirectories.

## Usage

```
./rm-trailing-whitespaces.sh [OPTION] [FILE|DIRECTORY]
```

## Options

- `-h, --help` : Display this help message.
- `-v, --version` : Display the script version.
- `FILE` : Remove trailing whitespaces from a specific file.
- `DIRECTORY` : Remove trailing whitespaces from all files in the specified directory and its subdirectories (excluding hidden directories like `.git`).
- No arguments : Asks for confirmation before removing trailing whitespaces from all files in the current directory and subdirectories.

## Installation

1. Download the script.
2. Make it executable:

```
   chmod +x rm-trailing-whitespaces.sh
```

3. Move it to a directory in your `PATH` (optional):

```
   mv rm-trailing-whitespaces.sh /usr/local/bin/
```

## Examples
- Remove trailing whitespaces from a file:

```
  ./rm-trailing-whitespaces.sh myfile.txt
```

- Remove trailing whitespaces from all files in a directory:

```
  ./rm-trailing-whitespaces.sh mydirectory
```

- Remove trailing whitespaces from all files in the current directory and subdirectories (with confirmation):

```
  ./rm-trailing-whitespaces.sh
```

- Display the help message:

```
  ./rm-trailing-whitespaces.sh --help
```

- Display the script version:

```
  ./rm-trailing-whitespaces.sh --version
```

## Notes

- The script skips hidden directories such as `.git`.
- It modifies files in place using `sed`.

## License

This project is licensed under the MIT License.