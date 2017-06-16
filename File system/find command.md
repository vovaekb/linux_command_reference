# Useful find commands
Look for all files in current directory
```bash
find
```
or
```bash
find .
```
Find only directories
```bash
find . -type d
```
Find only files within directory
```bash
find . -type f
```
List all the files of a specific directory
```bash
find /root
```
Find a file with name
```bash
find /opt/ros -name "setup.bash"
```
Find a file in multiple directories
```bash
find /usr/lib /lib -name "libflann*.so"
```
Find a file ignoring case
```bash
find /usr -iname "Flann*"
```
Find all file types other than the mentioned type
```bash
find . -not -name "*.txt"
```
Find files with using OR condition
```bash
find . -name "*.sh" -o -name "*.ini"
```
Find all the hidden files
```bash
find ~ -type f -name ".*"
```
Find all executable files
```bash
find . -perm /a=x
```
Find all empty directories and delete them
```bash
find . -type d -empty -exec rm -rf {} \;
```
