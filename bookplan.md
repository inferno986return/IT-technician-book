# IT technician book

A CompTIA/MCSA inspired book with plenty of information for getting your first job in IT. I recommend experimenting and have a practical chapter to familarise yourself with Windows Server.

The goal is to create a book that makes entering the world of IT easier. It's a general guide based off my own real-world experience and is not tied down to a particular certification though I am combining information from the CompTIA trifecta (A+, Network+, Security+), as well as several Microsoft certifications.

## Preface

## What is IT support?

* Zero, 1st, 2nd, 3rd line
* 

## Hardware chapter

### Monitor chapter

Monitors - refresh rate, sizes, TN, IPS, LCD, OLED, LED, DisplayPort (daisy-chaining and one cable), HDMI (each version of the HDMI spec has its own cable), size in inches, multi-monitoring instructions, overscan, running without a monitor is headless

### Keyboard chapter

* International Keybaord layouts - each country has one
* Alternative keyboard layouts - Colemak and Dvorak (Tip: The Dvorak keyboard has the fastest WPM when mastered.)
* Apple keyboard
* Membrane keyboards
* Mechanical keyboards
* Numpad
* Lock keys - Numlock, Scroll Lock, Caps Lock
* Text position keys - Home, End, Insert, Page Up, Page Down
* ISO Return vs ANSI Enter
* Super key (Winkey)
* Function key (fn)

### Power chapter

* AC and DC - use ~ for AC and...
* Kettle plug
* DC plugs
* Transformer (the cuboid box on a laptop charger for example)
* Watts, Amps and Volts
* Check the power requirements for a device
* Careful not to provide too much power as it can damage a device over time!
* Power Supply Units (PSU) - wattage, modular, semi-modular, non-modular, efficiency ratings (80+ bronze, etc.)

### Storage chapter

### CPU chapter

* RISC and CISC
* ARM, Intel, MIPS
* Frequency, cores, hyperthreading
* Virtualisation support

### RAM chapter

## E-mail chapter

* Open e-mail ports and protocols: POP3, IMAP, SMTP
* Proprietary e-mail ports and protocols: Exchange ActiveSync, MAPI
* Verify authenticity: SPF and DKIM
* Analysing headers (using MXToolbox.com)
* Out of space e-mails - check legitimacy at the webmail
* Configuring Outlook: adding accounts, shared mailboxes are mapped automatically...
* Troubleshooting Outlook: status bar, working offline, Outlook profiles, .pst and .ost files...
* Outlook for Mac
* Automatic replies

### Microsoft 365

* Check Office 365 webmail at: https://outlook.office.com/
* Set mailbox permissions
* Admin types

## Networking chapter

### Networking hardware
* Wi-Fi standard (IEEE 802.11) - WEP, WPA, WPA2, WPA3, TKIP, AES, a, b, g, n, ac, ag, 2.4GHz, 5GHz, channels
* Ethernet standard (IEEE 802.3) - RJ-45, CAT5, CAT5e, CAT6, CAT6a and CAT7
* Crossover and twisted-pair Ethernet cables
* Old cable standards: coaxial...
* Networking hardware (both commercial and SOHO variants): router, switch, hub, modem, PoE, EoP (powerline), firewall, IDS/IPS
* ~~Topologies: star, bus,~~
* Cellular: GSM

### Networking software
* TCP/IP and the OSI model - IPv4 (IP address exhaustion) and IPv6, subnet mask and the default gateway
* MAC addresses - 48 bit hexademical, IEEE register, ARP
* What is a protocol? - A set of rules between 2 or more devices, TCP and UDP, port numbers
* Common networking ports and protocols (tehnically any port and protocol could apply here): DNS, DHCP, ICMP, SNMP, HTTP, HTTPS, SIP...
* Common networking commands: `ipconfig`, `ifconfig`, `ping` (POSIX `ping` vs Windows `ping`), `pathping`, `traceroute` (and `tracert`), `host`
* DHCP and static IP addresses - leases, DORA,
* NAT - network address translation
* DNS - local DNS (hosts file), DNS servers (including Google's own 8.8.8.8 server), prerequisite of Active Directory
* Certificates 101 - how they work, prime numbers, advanced: concerns with Shor's algorithm beating certificates, TLS/SSL
* Pre-TCP/IP standarisation - NetBIOS, AppleTalk

## Printing chapter

* Printer cable - USB-B
* Common protocols: SMB,
* Drivers
* Wi-Fi printing
* USB printing
* Ethernet printing
* Types of printer (old CompTIA syllabus went crazy with printer types): inkjet, laser and thermal
* Simplex and duplex printing
* US letter paper size
* A paper sizes - A3, A4 - use the cool Fibonnaci-style diagram
* B paper sizes -
* Note: Both A and B paper sizes use the Lichtenberg ratio (not the Golden ratio as Persona 5 incorrectly states)
* CUPS and SMB printing

## Scanning chapter

* Scanner cable - USB-B
* TWAIN and WIA standards
* DPI
* Flatbed and feeder scanners
* OCR
* Scan to e-mail
* Scan to USB

## Filesharing chapter

* Common protocols: FTP, SFTP, FTPS, SMB, NFS, Bittorrent
* Centralised vs peer-to-peer (P2P) filesharing
* SMB/CIFS (and Samba) - as well as `net use` and `net share`, also creating a script that maps shares automatically
* NTFS permissions
* POSIX permissions - the dangers of `chmod -777`
* File servers
* NAS and SAN
* RAID

## Web server chapter

* LAMP stack
* Separate from a Windows domain environment
* Domain names

## Virtualisation

* Hyper-V - requirements, Gen 1 and Gen 2, .VHD and .VHDX, nested virtualisation (use matryoshka dolls for example)

## Installing Microsoft Windows

* Common protocols: TFTP
* Windows 10 and 11 editions - such as Home, Pro, Enterprise (KMS), Education (as well as end of life)
* Windows Server 2016 and 2019 editions - such as Essentials, Standard, Datacenter (as well as end of life)
* Minimum and recommended requirements
* Types of installation: zero-touch
* PXE
* Creating Windows images - WIM files, dism...

## Post-installation on Microsoft Windows

* Adding to an Active Directory domain on Windows 10 and 11 - GUI, PowerShell, CMD (if applicable)
* Creating a recovery USB - used to charge £30 for this at Currys/PC World.
* Reset Windows 10 and 11

## Installing Microsoft Windows applications

* Downloading software
* Microsoft Office - https://office.com/setup

## Introduction to Active Directory

* What is Active Directory?
* Forests, domains and child domains
* What is a domain controller?
* Active Directory suite - MMC snap-ins such as AD:CS, AD:UC, AD:SS, AD:DT, AD:AA...
* Active Directory objects - users, groups (security and distribution), printers, organizational units
* Active Directory recycle bin
* ADSIEdit
* Group Policy - policies and preferences, templates, Resultant Set of Policy, ordering with the LSDOU pneumonic, software installation (via .msi and .zapp files)
* Domain functional levels
* Maintenance tools -
* FSMO roles and the DRIPS pneumonic
* Client Access Licenses (CALs)

### Practical: Create a domain from scratch

Secondary school setup

### Practical: Created a shared folder

### Practical: Configure a Windows 10 computer, add to the domain and map the shared drive

## Shared-server

* Common protocols: RDP, VNC
* What is Citrix?
* Client Access Licenses (CALs)

## Troubleshooting Microsoft Windows

* Restart
* Running updates
* sfc /scannow
* Resetting network stack

## Glossary

## Bibliography

* References
* Further reading
I recommend the following books. Even though they are several years old, much of the information is still relevant:
  * [https://www.amazon.co.uk/dp/1326150251/](*Comptia Network+ V6 Study Guide - Indie Copy*) (2015), Matthew Bennett, lulu.com, ISBN-13: 978-1326150259
  * [https://www.amazon.co.uk/dp/8126562706](*Comptia A+ Complete Study Guide: Exams 220-901 and 220-902*) (2016, 3rd Edition), Quentin Docter, Emmett Dulaney, Toby Skandier, Wiley India Pvt., ISBN-13: 978-8126562701
  * [https://www.amazon.co.uk/dp/1509307842/](*Exam Ref 70-698 Installing and Configuring Windows 10*) (2018, 2nd Edition), Andrew Bettany, Andrew Warren, Microsoft Press, ISBN-13: 978-1509307845
  * [https://www.amazon.co.uk/dp/B06XS2R7T8](*Exam Ref 70-742 Identity with Windows Server 2016, First Edition*) (2017), Microsoft Press, Andrew Warren, ISBN-13: 978-0735698819

## Appendices
Mostly reference pages:

* Table of all the common ports and protocols
* NATO alphabet table
* Table of all the commands

## Planning notes

Question at the top: How can I get a 1st line IT support job?

Preface

Aggregate useful information from my own experiences and certifications. Even expired certifications can contain information that is both relevant and useful.

This book is not a substitute for 

Better main categories: Hardware, Networking, Microsoft Windows, Mac, GNU/Linux, Servers, Mobile Devices

NATO alphabet appendix

Use cbtnuggets for information.

Icon for old tech like a floppy disk?

Advanced: Supercomputer - Met Office and quantum computer

Hardware - motherboard, RAM, CPU, optical drive, fans (3-pin and 4-pin PWM), storage

Data recovery chapter - all I learnt including logical and physical recovery

Storage - SSD, HDD, Hybrid, eMMC, UFS, SMART, SATA, IDE,

Optical - CD, DVD, Blu-Ray

Update the licence key via Settings

Parted Magic

Mac section - what is macOS

GNU/Linux section - a different approach to computing

Old monitor adapters - VGA and DVI, also aspect ratios of 4:3, 16:9, 16:10, CRT

Virtualisation and setting up Windows Server, then Active Directory 101

What is WSUS?

Further reading - Introduction to Windows 10, Microsoft Server 2016, current CompTIA A+ book...

Udemy videos could be useful

Paper sizes - A3, A4, letter, thermal roll
Networking
Scanning - DPI, flatbed, feeder

Monitors - refresh rate, TN, IPS, LCD, OLED, LED, DisplayPort (daisy-chaining and one cable), HDMI (each version of the HDMI spec has its own cable), size in inches, multi-monitoring instructions, overscan, running without a monitor is headless

Types of firewall

Add A+ and Network+ ports and protocols

Common interview questions (that I experienced and Googled)

Common job criteria (Google them and adapt them into the book)

Backup section - incremental, differential, backup tape vs HDD, book vs scroll

MMC - Print Management

RODC, global catalog

Data wiping - Blancco, DBAN - Mersenne Twister

Outlook - rules and data policies

Win10 cert - GPT vs MBR, WindowsPE, dism...

MBAM checks for unauthorised commercial use

I need to look at the *For Dummies* books for inspiration. I'm thinking of using Material icons for infoboxes such as

* A lightbulb icon for tips to keep in mind such as a `ping` request may fail because a network firewall is blocking it, rather than the destination resource being unavailable
* An unlocked padlock icon for insecure technology such as HTTP and WEP.
* A warning triangle for dangerous procedures i.e. flashing BIOS and disassemmbling a PSU.
* A university cap for advanced information.

I can use black boxes with white text for terminal commands.

Start by adapting CompTIA and MCSA notes over on [Overleaf](https://www.overleaf.com/)), diary entries, any information that&#39;s relevant. I can also adapt college assignment material.

Quote: &quot;It takes the smartest individuals to realize there&#39;s always more to learn.&quot;

Quote: &quot;If I have seen further it is by standing on the shoulders of Giants.&quot;

Quote: &quot;Rosa Klebb: Training is useful, but there is no substitute for experience&quot;

Could have an xkcd comic such as this in the preface: https://xkcd.com/627/

Can I use old e-mails as a basis for real problems?

Use IT job descriptions as a basis

How to get a job in IT? 1st line support

Cover CompTIA basics but we can deviate into how to run a support desk.

What is an MSP?

Paper sizes - A3, A4, letter, thermal roll
Networking
Scanning - DPI, flatbed, feeder

Types of firewall

Add A+ and Network+ ports and protocols

E-mail protocols and examples, use Mozilla Thunderbird screenshots. Including POP3, IMAP, SMTP and Exchange ActiveSync, MAPI

Office 365 mailbox warning e-mails -> Check on https://outlook.office.com

Outlook troubleshooting and profiles

PXE booting and SCCM - zero touch, answer files, boot.wim, DISM, WindowsPE

Networking: TCP/IP, DNS, basic commands, firewalls (ping can be blocked), RDP/VNC

Everything is based off a metaphor such as drivers and servers

Remember the gym scenario from college which I can elaborate on it now.

Recommend: ITServiceDeskHelp (Zac), Professor Messer, textbooks (old ones are still useful)

SLAs, severity diagram (as defined by vmWare)

Hyper-V

Office 365...

How to get into IT?

CompTIA A+ and Network+ certifications, Microsoft certifications, M&C Saatchi,  

DNS

Server editions and CALs

Interview questions and scenarios:

* What is the difference between Windows Pro and Home
* What is the difference between TCP and UDP?
* A user isn't getting e-mail in Microsoft Outlook

Acknowledgements (for everyone)

Preface explaining motivations for this book including Jack Greenway, wanting to explain what I learnt in Curry&#39;s and having a practical use for my apprenticeship work… Maybe have an xkcd comic?

![](RackMultipart20210902-4-57ry8q_html_101b010171bd8f1a.png)

https://xkcd.com/627/

Soft skills such as logging tickets, phone etiquette, booking calendar, appointments, escalating issues within 15 minutes, learn the preferred communication style of your colleagues (we use Teams).

Split into theory and practical sections

FSMO roles, what they do, using `netdom query fsmo` to find the server that has them and moving or seizing them if needed. Use the DRIPS mneumonic.
https://docs.microsoft.com/en-us/powershell/module/activedirectory/move-addirectoryserveroperationmasterrole?view=windowsserver2019-ps

Use "Access Work or School" to remove and re-add account for Office login issues (particularly with inTune) for programs such as Outlook and Teams.

Remove troublesome profile from TS server by going to This PC -> System -> Advanced System Settings -> Advanced -> Profiles, then deleted the profile and re-login.

HP printer driver fix commands to reset print spooler and WIA driver respectively: `net start spooler && del %systemroot%\system32\spool\printers\*.shd && del %systemroot\system32\spool\printers\*.spl && net start spooler && sc config spooler depend=RPCSS` and `net stop StiSvc && sc config StiSvc depend= RpcSs/ShellHWDetection && REG add "HKLM\SYSTEM\CurrentControlSet\services\StiSvc" /v Start /t REG_DWORD /d 2 /f && net stop ShellHWDetection && REG add "HKLM\SYSTEM\CurrentControlSet\services\ShellHWDetection" /v Start /t REG_DWORD /d 2 /f && net start ShellHWDetection && net start StiSvc`

Symbolic links in Windows to move iTunes backup location

Setting up printer server, using Printer Management and Group Policy.

Troubleshooting printing on remote environments and ensure the printer is configured on local machine correctly.

Network commands such as: `ipconfig` and `ifconfig`, `ping`, `pathping`, `tracert`, `nslookup`, `arp`

Installing and updating Sage 50 Accounts, importance of backing up company data (to prevent a snowball effect of error growth), making a user account...

Setting up an Exchange server, setting alias, integrating with Active Directory, etc.

Out of space errors including on Outlook

Using WeTransfer to send files

ISPs such as TalkTalk have been known to block TeamViewer, AnyDesk, Chrome Remote Desktop and similar remote apps.

Cite quotes and sources. Watch IT Help desk channel

Check the drive space if Exchange mail flow is interrupted for all users.

1. Add space to the VM (in Hyper-V or VMware)
2. diskpart -> Scan - to show the unallocated space
3. Use Disk Management to extend the volume
4. Check the mail queue.
5. Send a test e-mail to check it's working

Create a contact in Exchnage to forward to an external address. https://exchangepedia.com/2008/02/how-to-forward-mail-to-an-external-email-address.html https://archive.ph/OD9jC

Types of servers: web, mail, domain controller, print, Terminal services, file, hypervisor, jumpbox…

Setting up a Terminal Services (ts) server, installing software (commands to run) such as Chrome for Enterprise

MMC Shared Folders snap-in and GPO

Group Policy 101 - mapping shared drives, mapping printers, installing software, disabling features, using custom templates for programs such as Chrome
http://woshub.com/deploy-printers-to-users-gpo/ https://archive.ph/Grk1H
https://server-essentials.com/support/deploy-and-install-printers-using-group-policies

BSOD troubleshooting using BlueScreenView and searching the stop code. Windows kernel panic

Appendix with the useful Command Prompt/PowerShell/Bash commands.

Recovery USB

Using a password manager to store the passwords for each client.

LibreOffice Vs OpenOffice, for when you need a suite...

Ensure software is licenced for commercial use. Explain Malwarebyte&#39;s proactively looking for EULA-breakers, you don&#39;t need WinRAR (use 7-Zip)... A great site is TLDRLegal for simple explanations of common software licences: https://tldrlegal.com/

I&#39;ll explain all the licencing for the software in this book.

Introduction to 3CX. Setting it up...

Booking a manufacturer repair (either under the 1 year warranty or extended warranty), get the serial number, ensure user data has been backed up (and they are aware of data loss). Explain where to find serial number (also Dell call them service tags) by looking for label or running command &quot;wmic bios get serialnumber&quot; and it&#39;s PowerShell equivalent.

Have a focus on troubleshooting issues such as network connection, system instability, changing passwords, Office 365, Active Directory, adding computers to the domain and renaming them…

Use GUI and PowerShell methods.

Peripherals such as monitors (IPS vs TN, cables, LCD/LED/CRT...), keyboards (layout, keys, membrane, mechanical), mouse (trackball, laser, wired, wireless), USB/PS2.

Serial Vs parallel such as SATA Vs IDE.

Outlook overriding PST/OST file size in Registry Editor, enabling/disabling caching, calendar permissions, updating offline address book, signature, configuring user interface (fonts, panes, disable automatically marking e-mail as read,)...

Remove WSUS from Registry Editor and common troubleshooting tips for Windows Update, including stopping &quot;bits&quot; and &quot;wuauserv&quot; (via services.msc and PowerShell), renaming &quot;SoftwareDistribution&quot; and starting them back.

Office 365 troubleshooting including message trace. Also, escalating to Microsoft/cloud provider

RDP files and connecting to another computer/server such as RDS gateway and redirection. Show configuration settings for Windows, macOS and Linux. Discuss Royal and Microsoft Remote Desktop (orange icon).

DNS, DNS records (A, MX...), setup and configuring a DNS server (on Windows Server and Linux), DNS filtering, host file (on Windows and other operating systems), DNS issues over VPN with Drayter Vigor routers

VPN with built-in and Smart VPN Client, FortiClient VPN + different types of protocols (PPTP, L2TP, SSTP) on Draytek and RAS. Different VPN errors (such as PPP control errors, remote dial-in), DHCP

Outlook calendar sharing

M&amp;C Saatchi - Warranty checking, PXE boot installation, Secure Boot, BitLocker...

Currys/PC World - Reset this PC, installing Office and McAfee, running updates, creating a recovery USB, nuking a computer for WEEE using Blancco (or Darik&#39;s Boot and Nuke, I recommend Parted Magic)…

HDDscan and using a HDD caddy

CCleaner, Advanced System Care and Malwarebyte&#39;s...

Section on…

Using TeamViewer and AnyDesk, particularly setting it up on Mac (https://community.teamviewer.com/English/kb/articles/44699-how-to-control-a-mac). Also demonstrate connecting, setting up unattended access, redirected printing,

Soft skills, setting up a software update or installation. Taking a snapshot on the hypervisor (vmware untick memory cache)...

Reset your local account password using reset disk and WIndows 10 install USB. https://www.pcunlocker.com/reset-windows-10-password-with-install-disk.html

Setting up return receipts, out of office... in Outlook, if you need them.

Office 365 forwarding, out of office, etc.

Windows 10 Pro N vs Pro

Configuring SharePoint and OneDrive on Office 365 with a new site. Sync to OneDrive with the &quot;Sync&quot; button

Granting Office 365 mailbox permissions to accounts, such as shared mailboxes and user accounts

Troubleshooting Hyper-V, replication…

Access point clustering

Setting up RDP files, RDP 101

The whois and host commands in Bash via WSL

Multi-monitoring using Settings to change the screen order and Win+P to duplicate/extend. Explain the limitations of remote troubleshooting this over TeamViewer/AnyDesk.

Setup wireless access point: SSID, PSK (WEP/WPA/WPA2), a/b/g/n/ac/, MAC filtering, VPN (PPTP, L2TP/L2TP over IPsec/SSTP/…), NAT, IPv4 vs IPv6.

Installing Microsoft Office (perpetual vs Office 365), entering the key at https://office.com/setup...

Reset TCP/IP stack…

[https://kb.wisc.edu/dermatology/page.php?id=31480](https://kb.wisc.edu/dermatology/page.php?id=31480)[https://archive.ph/kMe0t](https://archive.ph/kMe0t)

1. In the search box on the taskbar, type Command prompt, press and hold (or right-click) Command prompt, and then select Run as administrator \&gt; Yes.
2. At the command prompt, run the following commands in the listed order, and then check to see if that fixes your connection problem:
3. Type netsh winsock reset and press Enter.
4. Type netsh int ip reset and press Enter.
5. Type ipconfig /release and press Enter.
6. Type ipconfig /renew and press Enter.
7. Type ipconfig /flushdns and press Enter.
8. Restart computer.

Client network outage checklist

**Network outage checklist:**

1. Confirm the situation is a network outage by asking if the issue affects multiple users or just one.

1. Ask users to perform network troubleshooting commands such as ipconfig (or ifconfig) and ping. As well as checking access to shared drives. This may also be a DNS issue, so check which DNS server the computer is using and possibly the hosts file as well.

1. Restart the router by removing power for 10-15 seconds.

1. Escalate to the internet service provider by checking an outage map or calling their support line to request a line test. You may need to check you are a registered contact with the client and have them add you to their account.

Adding RAM and disk storage to Hyper-V and VMware ESX. Using Disk Management and Powershell.

Cover old and new topics. Prioritise new

Preface explaining how I got into IT and my motivations for this book

Active Directory setup example with 2 domain controllers, home drive, teacher&#39;s resources, student drive for Woolton Hall School in Merca novels.

  - Windows 10
  - Editions (Home, Pro, Enterprise, Education, OEM, Workstations)
  - Upgrading from Windows 7 (show which edition goes to which)
  - Activating a Windows 10 key (via Settings or slmgr.vbs)
  - Making a recovery flash drive
  - Maintaining and troubleshooting Windows 10
    - Running slow (check resource use on Task Manager and Resource Monitor, use Event Viewer to look at logs)
    - Check system specs (with System Information and Speccy)
    - Safe Mode (and using msconfig)
    - Check and repair hard disk errors (with chkdsk /r /f)
    - Removing malware (with Malwarebytes Anti-Malware)
    - Removing unnecessary files (with Disk Cleanup and CCleaner)
    - Defragmentation and optimisation (with Disk Defragmenter and Defraggler)
    - Verify Windows 10 integrity (with sfc /scannow, dism -checkhealth, )
    - Rebuild user profile (with Registry Editor)
    - Windows updates
  - Reset Windows 10
  - Enabling BitLocker (via GUI, then PowerShell)
  - Connect to VPN (via Windows Settings or Draytek Smart VPN)
  - Map a network drive (via GUI, then Command Prompt and PowerShell)
  - Administrative Tools
    - MMC
      - Disk Management
      - Local Users and Groups - Making an account, promoting an account to administrator…
      - Services (services.msc)
    - Task Manager
    - Registry Editor (regedit)
    - System Configuration (msconfig)
  - Hyper-V
    - Introduction to Hyper-V (.vhd/.vhdx..)
    - Prerequisites (find via sysinfo or System Information)
    - Installing Hyper-V (via GUI/PowerShell)
    - Create a virtual machine (step-by-step, Gen 1 vs Gen 2)
  - Enabling Windows Subsystem for Linux (via GUI and PowerShell)
    - Install and configure Windows Terminal
    - Change default directory for WSL
  - Connecting an XBOX One or XBOX 360 gamepad
    - Game Bar
- Microsoft Office
  - Editions
  - Deploying Office 365
  - Administration of Office 365
    - User management
    - Mailboxes
    - Licences
    - …
    - eDiscovery
    - Mail flow
    - Spam filter
  - Microsoft Outlook
    - Recreating Outlook profile (via Control Panel → Mail (32-bit))
    - Downloading all/some of the mail from the server
    - Setting up rules for folders (be careful of malicious rules)
    - .pst, .ost and .ics files
    - Recalling a sent e-mail
- Windows Server 2012+ (what isn&#39;t EOL)
  - Editions (Foundation, Essentials, Datacenter)
  - CALs
  - Introduction to domains, trees and forests.
  - Server Manager
  - MMC
  - Create a domain controller server using Active Directory: Domain Services (AD:DS)
  - Active Directory: Users and Computers (AD:UC) - (reset a password takes 15 minutes).
  - NIC teaming
  - Setting up a VPN (Enable Dial-in), MS-CHAP, - some VPNs use LDAP others need configuring on the router. Remote Access ports to set the maximum allowed connections… Using built-in, Draytek Smart VPN, Cisco...
- Networking
  - What is a switch, access point, router
  - IP conflicts – IP Scanning (use the Advanced IP Scanner)
  - Reset network stack (when you are having issues connecting to the internet and there&#39;s no obvious reason why)
- Printing
  - Laser, inkjet and thermal.
- Security
- Hardware
  - Hard disks
    - Cloning (with Clonezilla)
    - Data recovery
    - S.M.A.R.T. checking
- Miscellaneous
  - Warranties (1 year manufacturer&#39;s warranty and extended warranties) - hard drive warranties are 2 years.
- Appendices (Windows hotkeys, useful commands…)
  - Hotkeys (Windows, macOS, GNU/Linux)
  - Command-line programs (Windows, macOS and GNU/Linux)
  - Recommended software
    - Piriform (CCleaner, Defragler, Recuva, Speccy)
    - Advanced IP Scanner
    - Belarc Advisor
    - MBAM
    - Brave
    - CrystalDiskInfo
    - CPU-Z
    - GPU-Z
    - Citrix Receiver/Workspaces
    - Draytek Smart VPN
    - TeamViewer
    - AnyDesk
    - TightVNC
    - TreeSize Free
    - HeavyLoad?
    - Windows Terminal
    - BlueScreenView
    - Speedfan
    - 7-Zip
    - FortiClient
    - mRemoteNG
    - Intel Processor Diagnostic Tool
    - Memtestx86
    - PortQuery
    - Vendor utilities - HP Support Assistant, Dell SupportAssist, Lenovo Vantage, myASUS
  - Common protocols and default port numbers
  - Interview questions for 1st line
    - Difference between Windows 10 Home and Pro
    - TCP and UDP
    - What is Active Directory?
    - What is subnetworking (subnetting)?
    - How would you prioritise these tickets?
  - NATO phonetic alphabet table
  - Common ports and protocols table
  - Windows 10 hotkeys
- Bibliography and further reading (Cite CompTIA and MCSA textbooks, along with Matthew Bennett&#39;s book and IT career questions)
- Index

[MXtoolbox](https://mxtoolbox.com/) - check MX headers to find original sender

[Have I been pwned](https://haveibeenpwned.com/) - check to see if the account has been compromised

SecureCRT

MobaxTerm

Wireshark

qBittorrent

WinSCP

Notepad++

Cisco Packet Tracer

WinSCP/FileZilla

Putty

Postman

MOSH

Docker

Electricty 101 - what are AC / DC, as well as Volts, Amps and Watts? Especially in the context of computing. As well as unintteruptible power supplies.

What did I do at Virtual Tech, how did I get in the role via apprenticeship?

**Acknowledgments**

CompTIA

JustIT

The Knowledge Academy

MBit Training

3AAA