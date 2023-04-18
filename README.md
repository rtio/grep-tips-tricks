# grep tips and tricks

A few tips and tricks

## Basic Grep Usage

```bash
grep 'error' /path/to/your/logfile.log
```

This will output any lines in the specified log file that contain the word "error."

## Case-Insensitive Searching

```bash
grep -i 'error' /path/to/your/logfile.log
```

This command will match lines containing "Error," "ERROR," and any other combination of upper and lowercase letters.

## Using Regular Expressions

```bash
grep -E '([0-9]{1,3}\.){3}[0-9]{1,3}' /path/to/your/logfile.log
```

The '-E' flag tells grep to use extended regular expressions, which offer more powerful pattern-matching capabilities.

## Invert Matching

```bash
grep -v 'debug' /path/to/your/logfile.log
```

This command will output all lines that do not contain the word "debug."

## Displaying Line Numbers

```bash
grep -n 'error' /path/to/your/logfile.log
```

This command will show the line number before each matching line, making it easier to locate the source of an issue.