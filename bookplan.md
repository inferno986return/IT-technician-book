# IT technician book

Start by adapting CompTIA and MCSA notes over on [Overleaf](https://www.overleaf.com/)), diary entries, any information that&#39;s relevant.

Quote: &quot;It takes the smartest individuals to realize there&#39;s always more to learn.&quot;

Quote: &quot;If I have seen further it is by standing on the shoulders of Giants.&quot;

Quote: &quot;Rosa Klebb: Training is useful, but there is no substitute for experience&quot;

Acknowledgements (for everyone)

Preface explaining motivations for this book including Jack Greenway, wanting to explain what I learnt in Curry&#39;s and having a practical use for my apprenticeship work… Maybe have an xkcd comic?

![](RackMultipart20210902-4-57ry8q_html_101b010171bd8f1a.png)

https://xkcd.com/627/

Soft skills such as logging tickets, phone etiquette, booking calendar, appointments, escalating issues within 15 minutes, learn the preferred communication style of your colleagues (we use Teams).

Split into theory and practical sections

Network commands such as: ipconfig, ping, pathping, tracert, nslookup

Setting up an Exchange server, setting alias, integrating with Active Directory, etc.

ISPs such as TalkTalk have been known to block TeamViewer, AnyDesk, Chrome Remote Desktop and similar remote apps.

Cite quotes and sources. Watch IT Help desk channel

Types of servers: web, mail, domain controller, Terminal services, file, hypervisor, jumpbox…

MMC Shared Folders snap-in and GPO

Group Policy 101 - mapping shared drives, installing software, disabling features, using custom templates for programs such as Chrome

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

Outlook overriding PST/OST file size in Registry Editor, enabling/disabling caching, calendar permissions, updating offline address book, signature...

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

Using TeamViewer and AnyDesk, particularly setting it up on Mac. Demonstrate connecting, setting up unattended access, redirected printing,

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

**Acknowledgments**

CompTIA

JustIT

The Knowledge Academy

MBit Training

3AAA