# Bash Cheatsheet

List all processes running
```ps -afux```

Display folder content
```ll```

Display content of file
```more``` or ```cat```

List of logged-in user
```w```

List network interfaces
```ip a```

Change owner of file
```chown OWNER[:GROUP] FILE```
```chown :GROUP FILE```

Change owner of current directory recursively
```chown OWNER:GROUP . -R```

Change permission of file
```chmod 2775 . -R```

| #   | rwx                | Permission |
| --- | ------------------ | ---------- |
| 7	  | 4(r) + 2(w) + 1(x) | rwx        |
| 6	  | 4(r) + 2(w)        | rw         |
| 5	  | 4(r) + 1(x)        | r-x        |
| 4	  | 4(r)	           | r--        |
| 3   | 2(w) + 1(x)        | -wx        |
| 2   | 2(w)               | -w-        |
| 1   | 1(x)               | --x        |


setgid on directory : all the newly created files in this directory belong to the directory's owning group 

First digit of chmod sequence
```
setuid=4
setgid=2
sticky=1
```
