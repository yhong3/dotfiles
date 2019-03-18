Print file count in subdirectories 
```du -a | cut -d/ -f2 | sort | uniq -c | sort -nr```
