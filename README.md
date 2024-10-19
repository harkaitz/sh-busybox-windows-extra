BUSYBOX WINDOWS EXTRA SCRIPTS
=============================

Scripts for Busybox for windows.

## Help

schtasks-boot

    Usage: schtasks-boot [-V] TASK COMMAND
    
    Schedule a shell command to be executed at boot using the windows
    schtasks utility. The task name will be prepended "BOOT-".
    
    Default shell: C:\Windows\System32\sh.exe ($SCHTASKS_SHELL)

schtasks-daily

    Usage: schtasks-daily [-V][-t HOUR] TASK COMMAND
    
    Schedule a task named "DAILY-<TASK>" to be executed daily,
    by default at "2:00".
    
    Default shell: C:\Windows\System32\sh.exe ($SCHTASKS_SHELL)
    Default hour: 2:00 ($SCHTASKS_HOUR)

schtasks-list

    Usage: schtasks-list ...
    
    Manage scheduled tasks with schtasks-{daily,boot}(1).
    
      -l              : List created tasks.
      -d TASK         : Disable tasks.
      -r TASK         : Execute tasks.
      -L TASK         : Print log.
    
    Tasks that start with "BOOT-" and "DAILY-" are listed.

wsudo

    Usage: wsudo [-u USER] COMMAND
    
    Execute command elevated using the local SSHD server to do the
    elevation.

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
