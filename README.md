### Change all directory permission to 755 in current directory and subdirectory
```sh
find . -type d -exec chmod 755 {} \;
```

### Change all file permission to 644 in current directory and subdirectory
```sh
find . -type f -exec chmod 644 {} \;
```

### Search all occurrence in a directory and subdirectory and replace
```sh
find . -type f -exec sed -i -e 's/SEARCH/REPLACE/g' {} \;
```

### FTP Directory download with wget
```sh
wget -m ftp://USERNAME:PASSWORD@HOSTNAME/path/to/directory
```

### Word, line, character counts in a file
```sh
wc filename // words, lines and chars
wc -w filename // words
wc -l filename // lines
wc -m filename // chars
```

### Truncate/remove lines in a file
```sh
sed -i <start>,<end>d filename
sed -i 10,100d file.txt // remove lines from 10 to 100 line number
```
