# serve
Instant, backgrounded local hosting for multiple files and folders.

Requires python.a

# usage

```bash
# serve the current directory foo:
serve .
# link copied to clipboard, e.g.
# http://192.168.0.6:3942/foo

# serve some more files...
serve ../bar/file1.txt ../bar/file2.txt
# file1.txt and file2.txt additionally hosted

serve -c
# all served items cleared up
```

![example serve result](screenie.png?raw=true "example serve result")

# how
serve starts a python simplehttpserver running out of ~/.pythonserver. Files and folders are then symlinked from that directory as and when you need them.
