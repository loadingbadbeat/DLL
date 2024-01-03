# DLL
Everything DLL


<b>New DLL Hijacking Technique Let Attackers Bypass Windows Security</b>

DLL hijacking is a technique where a malicious DLL (Dynamic Link Library) is placed in a directory that a vulnerable application searches before the legitimate one. 

When the application is launched, it unknowingly loads the malicious DLL instead, allowing attackers to:-

Execute arbitrary code
Compromise the system

Recently, the cybersecurity researchers at a multi-layered incident response company, Security Joes, discovered a new DLL hijacking technique that enables threat actors to bypass Windows mechanisms.

<b>New DLL Hijacking Technique</b>

This new technique exploits trusted WinSxS executables using DLL Search Order Hijacking. 

This enables threat actors to execute malicious code within Windows folders, which eliminates the need for extra binaries. 

Besides this, it’s compatible with both Windows 10 and 11, as it bypasses high privilege requirements.

The DLL Search Order Hijacking exploits how Windows apps load DLLs, taking advantage of those without specified file paths. 

Threat actors manipulate apps depending on predefined search orders that place a malicious DLL in a prioritized directory. 

Many methods for this require apps not to specify full paths, often due to development oversights.

Knowing how Windows loads DLLs and executables is one of the key things, and the system follows a sequence during the loading process.

This ensures efficient operation by locating necessary components like DLLs. Not only that even, it also provides an alternative method for finding resources.

Besides this, the Windows OS flow for searching and loading resources includes the following things:-

Application’s launch directory<br>
C:\Windows\System32<br>
C:\Windows\System<br>
C:\Windows<br>
Current working directory<br>
Directories in the system’s<br>
User’s PATH variables<br>

Exploiting the loading process lets threat actors inject unauthorized code into the trusted processes, which helps in deceiving the:-

Security tools<br>
Security experts/analysts

This new malicious technique is completely sophisticated and stealthy as it enables threat actors to achieve several types of malicious goals like:-

Compromise systems<br>
Evade detection

The WinSxS folder is a critical component in Windows OS at “C:\Windows\WinSxS.” This vital component crucially maintains multiple versions of system files. 

Not only that even, it also preserves previous versions during updates, which causes the folder to grow with each update for the Windows operating system.

![image](https://github.com/loadingbadbeat/DLL/assets/45952458/04933592-2fbf-4b34-b2ed-a02cfd24d8b0)

Here below, we have mentioned all the key purposes of the WinSxS folder:-

Version Management<br>
System Integrity<br>
Dynamic Activation<br>


<b>Advantages New DLL Hijacking Technique</b>

Here below, we have mentioned all the key advantages of this new DLL hijacking technique:-

Circumventing High Privilege Requirements</br>
Eliminating the Need for Additional Binaries</br>
Enhancing Stealth</br>
