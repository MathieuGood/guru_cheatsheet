# Bash Cheatsheet

Execute command before another with "`"
```echo hello `whoami` ```

Start process in the background with "&"
```vi &```

Suspend process
```Ctrl + Z```

Go back to process
```fg```

All processes of current user
```ps a```

All processes of all users
```ps aux```

All processes in a tree
```psstree``

Find "apache" process
```ps aux | grep apache```

Create file with text in it with '>' or '>>'
```echo "Adds text and overwrite current file if exists" > test.txt```
```echo "Adds text and concatenates it to the current file if exists" >> test.txt```

Create file to get error message with '2>'
```echoooo "There is an error in the command" 2> error.txt```

Create file with current vi processesm, replace spaces by ; and write to file
```ps | grep vi | tr " " ";" > process_list.csv```

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

```chmod u=rwx,g=rx,o=r myfile.txt```

First digit of chmod sequence 
```
setuid=4
setgid=2
sticky=1
setgid on directory : all the newly created files in this directory belong to the directory's owning group 
```

Folders
``` 
/etc > config files
/usr > User specific files
/home > User folder
/var/logs > Log files
/bin > Applications
/sbin > Applications 
```

Stop/start/restart service
```
sudo systemctl stop SERVICE_NAME
sudo systemctl start SERVICE_NAME
sudo systemctl restart SERVICE_NAME
```

List network devices
```nmap -sP 192.168.1.0/24```

Find files and directories
```find -name *gold*```

Case insensitive search
```find -iname *gold*```

https://www.linuxtricks.fr/wiki/find-rechercher-et-bien-plus