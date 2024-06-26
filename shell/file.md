__count the number of lines in a file__
```shell
wc -l filename
```

wc is the word count command.
-l flag tells to count the number of lines in the file.

__search for a string within a directory and its subdirectories. Limit the search to specific file types.__
```shell
find . \( -name "*.md" -o -name "*.txt" \) -exec grep -l "Hello, world!" {} \;
```
__copy the first 10 lines from a file to a new file__
```shell
head -n 10 input.txt > output.txt
```

__search for a file with part of its name within a directory and its subdirectories__
```shell
find /search_dir -name '*partialname*'
```
__search for files that contain an input string__
```shell
grep -r "my_string" /search_dir
```

__search within files with an extension__
```shell
grep -r --include="*.extension" "my_string" /search_dir
```

__move all files except a few files__
```shell
find /source/directory -type f -not -name 'file_to_exclude1' -not -name 'file_to_exclude2' -exec mv {} /destination/directory \;
```

__search a string within a file__
```shell
grep "mystring" filename
```
