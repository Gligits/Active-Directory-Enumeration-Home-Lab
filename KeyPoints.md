
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

 ### What is active directory
 Active Directory (AD) is a directory service developed by Microsoft for Windows domain networks. 
 It is a centralized database that manages and stores information about users, computers, and other resources within a 
 network. 
 AD allows administrators to manage permissions and control access to network resources. It also supports authentication and 
 authorization, ensuring that only authorized users can access specific resources.
 ### What is the purpose of the enumeration
 Enumeration is the process of gathering information . The purpose of enumeration is to identify and list resources, such as 
 user accounts, network shares, services, and other network components, which can then be used for further analysis or 
 exploitation. 
 In cybersecurity, enumeration is often used by attackers during the reconnaissance phase to identify potential 
 vulnerabilities or entry points in a system.
 ### creating the environement 
 We’re going to create a lab environment where you can safely test and experiment with configurations/attacks. This setup 
 will include virtual machines and network configurations, allowing us to simulate real-world scenarios.

# Architecture and Environment setup

We require two server machines and one client machine. Utilize VMware and enable bridged networking for all of them. If any machine is on another laptop, bridge it and assign it an IP address within the same network as the other machines ( the host machine firewalls needs to be disabled )


![Frame 1 (2)](https://github.com/user-attachments/assets/6c0ed96c-d0c2-43d5-8980-b1e5f738bab5)



### Activating AD DS  on the servers 
### Promoting the Parent Domain (Forest Root)
### Promoting the Child Domain (Adding to the Forest)
  *  Ensure the IP address of the client is within the same network as the parent domain's IP address.
  * Set the DNS of the client to the IP address of the parent domain.
  * Test the connectivity by pinging the parent domain.

### Common Issues and Troubleshooting
If the ping test fails:
  * Check the firewall settings to ensure ICMP traffic is allowed.
  * Verify that both machines are using the same network bridge.
  * If the machines are on different hosts, check the host firewall settings.
  * If a new client machine is created for the forest enumeration, ensure that the time and date are synchronized with the other server machines to allow proper forest enumeration.
  * When promoting a child domain as a subdomain of the parent, use the format: name_of_the_domain\Administrator

    
### adding the client to the server 



--> Note that the necessary  machines  should stay powered on when doing this operation
--> when using different machines 
![Frame 2 (1)](https://github.com/user-attachments/assets/6e017f77-e7cc-4955-8599-c36440c93e08)


   
# Tools and Techniques  





