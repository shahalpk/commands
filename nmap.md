
**To scan all TCP ports if PING is blocked (better use this always)**

    nmap -Pn -sU -p0-65535 <IP ADDRESS>


**To scan all UDP ports if PING is blocked (better use this always)**
    
    nmap -Pn -sT -p0-65535 <IP ADDRESS>
