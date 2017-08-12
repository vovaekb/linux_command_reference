# Useful grep commands
Find all occurrences of specific word in files corresponding to some pattern (e.g., text files):
```bash
grep -i promo -H `find . -name *.txt -print`
```
