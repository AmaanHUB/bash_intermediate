# Bash And Linux Cheat Sheet

Some common commands and some intermediate topics.

* **Everything is a file**
* File extensions don't matter, only really needed for people
* Case sensitive

## Some Useful Commands
```sh
# shows the type a file is
file <file_name>
```


## Stderr, Stdout, And Stdin

To capture stderr, stick a `2` in front of the streaming symbol and a `1` just for stdout .e.g.
```sh
# if file_name doesn't exist, will be appended only if it doesn't exist
ls file_name 2>> error_logs.txt

# redirect stdout and stderr
ls file_name 2>&1 output_and_errors.txt
```
