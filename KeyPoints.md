
                               _   _             _____  _               _                    
                     /\       | | (_)           |  __ \(_)             | |                   
                    /  \   ___| |_ ___   _____  | |  | |_ _ __ ___  ___| |_ ___  _ __ _   _  
                   / /\ \ / __| __| \ \ / / _ \ | |  | | | '__/ _ \/ __| __/ _ \| '__| | | | 
                  / ____ \ (__| |_| |\ V /  __/ | |__| | | | |  __/ (__| || (_) | |  | |_| | 
                 /_/    \_\___|\__|_| \_/ \___| |_____/|_|_|  \___|\___|\__\___/|_|   \__, | 
                                                                                       __/ | 
                                                                                      |___/  
                     




# List of content 

[Overview](#overview)

[Environment Setup](#architecture-and-environment-setup)

[Tools and Techniques](#tools-and-techniques)

# Overview   

 * What is active directory
 * What is the purpose of the enumeration
 * creating the environement 

# Architecture and Environment setup

We require two server machines and one client machine. Utilize VMware and enable bridged networking for all of them. If any machine is on another laptop, bridge it and assign it an IP address within the same network as the other machines ( the host machine firewalls needs to be disabled )

![Frame 1](https://github.com/Nirsen/Active-Directory-Enumeration/assets/88287290/c65ec16a-3316-40a6-b054-d1f739e73f6b)


## Activating AD DS  on the servers 
## Promoting the father's domain ( as a forst ) 
## Promoting the son's domain ( adding it to the forest )
  *  the ip adderss of the client should be in the same network as the father's ip adress
  *  the dns of the client is the ip address of the father
  *  testing the ping first
  *  some problem that u can encounter :  if the ping doesnt work then checking the firewall if it accepts icmp analyse then checking that the two machines are uding the bridge , if the machines are on different hosts then checking the host firewall
    
## adding the client to the server 



--> Note that the necessary  machines  should stay powered on when doing this operation
--> when using different machines 
![Frame 2](https://github.com/Nirsen/Active-Directory-Enumeration/assets/88287290/5224a4fd-3bdb-40fc-bc90-3da77cb1d447)

   
# Tools and Techniques  





