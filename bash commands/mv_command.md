# Bash Command: mv
The `mv` command in Bash is used to move or rename files and directories. Its basic syntax is as follows:

## Syntax

```bash
mv [options] source destination
```

## Usage Examples

1. Move a file to a different directory:

```bash
mv file.txt /path/to/destination/
```
This command moves the file `file.txt` to the directory specified by `/path/to/destination/`.

2. Rename a file:

```bash
mv old_name.txt new_name.txt
```
This command renames the file `old_name.txt` to `new_name.txt` in the same directory.

3. Move and rename a file simultaneously:

```bash
mv old_name.txt new_name.txt
```
This command moves the file `file.txt` to the directory specified by `/path/to/destination/` and renames it to `new_name.txt` in the new location.

4. Move multiple files to a directory:

```bash
mv file1.txt file2.txt /path/to/destination/
```
This command moves multiple files (`file1.txt` and `file2.txt`) to the directory specified by `/path/to/destination/`.

5. Move a directory to a different location:

```bash
mv directory /path/to/destination/
```
This command moves the entire directory `directory` to the specified destination directory.

6. Overwrite existing files:

```bash
mv -f source destination
```

The `-f` option forces the move, even if a file with the same name already exists in the destination directory. This will overwrite the existing file.

> Note: The `mv` command can also be used to move and rename directories, and it can accept various options to modify its behavior. Refer to the `mv` command's man page (`man mv`) or use the `mv --help` command for more information.



