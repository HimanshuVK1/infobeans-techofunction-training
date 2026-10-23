Day5 23/10/26    
    
Windows Processes & Services

Processes
Threads Services
Service dependencies
Windows Services console
Task Manager
Resource Monitor
CPU troubleshooting
Memory troubleshooting
Service startup failures
Service recovery

====================================================================
Process vs Program
dxdiag 
<img width="729" height="528" alt="image" src="https://github.com/user-attachments/assets/7c14f460-6d50-4978-92dc-9903ae21ff3b" />

Types of Processes:
1) Foreground: It uses 80% of cpu and gpu resources
2) Background: It uses 20% of cpu and gpu resources

-----------------------------------------
python code for 
    import threading, time
    
    def task(n):
        print(f"Task {n} started")
        time.sleep(2)          # simulates waiting (API/DB call)
        print(f"Task {n} done")
    
    start = time.time()
    threads = [threading.Thread(target=task, args=(i,)) for i in range(4)]
    for t in threads: t.start()
    for t in threads: t.join()
    print(f"Total: {time.time() - start:.1f}s")   # ~2s, not 8s

===========================================

Process vs. Daemons
Service==============>daemon
Restart/Reload
---------------------------
100 request
True positive /False positive                                             True               False
Triage is a practices to prioritize to requirement.
https://www.bing.com/videos/riverview/relatedvideo?q=false+positive+in+monitoring+devops+explain&mid=0C2C1D146E8356321C140C2C1D146E8356321C14&churl=https%3a%2f%2fwww.youtube.com%2fchannel%2fUCFMdEr1H3hhCIdoKwsK80Tw&FORM=VIRE

event=====>incident

logs===>low level
event========>high level

Logs/event
severity/priority================>
source===================>who

==============================================================
Command                                 Purpose
Get-Process                                    Lists running processes
Get-Service                                     Lists services
Get-CimInstance Win32_Process    Retrieves process details
Get-CimInstance Win32_Service    Retrieves service configuration and status
Get-Counter                                         Reads performance counters
Get-WinEvent                                        Reads Windows event logs
Start-Service                                         Starts a service
Stop-Service                                       Stops a service
Restart-Service                                   Restarts a service
Set-Service                                          Changes supported service settings
Get-Process -Id                                   Inspects a process by PID

