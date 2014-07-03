
## Introduction to Command Line Interfaces

Before the graphical user interface (GUI), a
command line is how users interacted with computers.
To take up the command line is about like switching
from an automatic transmission to a manual transmission
with a stickshift. On the command line, you have 
more power, but you must learn to use a command
line well to take on more responsibility. Instructions
below assume that you are an Administrator on your
operating system and/or that you have selected to
run a routine in the Administrator mode.

Windows had two different command line interfaces,
MS-DOS (command.exe or cmd.exe) and PowerShell
(powershell.exe). MS-DOS ships with all versions of
Windows, but PowerShell may need to be installed.

Modern Macintosh computers (beginning with OS X) are 
a UNIX-based operating system. When you launch the
terminal, you have access to full range of UNIX commands.
Much online advice for open-access software presumes
that you know how to access and use the command line
and that you know UNIX commands also work in on Macintosh
computers.  


## About Windows Command Line Tools

Many PowerShell advantages over MS-DOS concern
networking and system administration, which you
are unlikely to need in this course, but two important advantages
of PowerShell are that it is more like UNIX command line
and has an Administrator mode. On Windows 7 and later,
MS-DOS may be denied access to system folders or commands.
Many command line options that you are asked to perform 
may also work on MS-DOS, but some will require PowerShell.

### Checking if PowerShell is installed
 - On the Start menu search box, type "PowerShell."
 - If not application is availalbe, see "Installing Windows PowerShell"
   below.
 - You may have two PowerShell options: "Windows Powershell"
   and "Windows PowerShell (x86)." If you have both, use the
   plain "Windows PowerShell." Ignore the options for ISE
   or Modules.
 
### Installing Windows PowerShell
PowerShell is part of the "Windows Management Framework 3.0" (WMF).
 - If PowerShell is not already installed, you may install the
   WMF at [http://www.microsoft.com/en-us/download/details.aspx?id=34595](http://www.microsoft.com/en-us/download/details.aspx?id=34595).
 - If you are unsure whether you have 32-bit or 64-bit windows,
   search for "System Information" on the Windows Start search box.
   In the System Information dialog, under System Summary (default display),
   search for "System Type." You will either have an "x86" or "x64" PC.
 - Select for download the 32-bit (x86) or the 64-bit (x64) system,
   and double-click the downloaded file to run the installation.

### Running PowerShell
 -  On the Start menu search box, type "Powershell" and right-click
    the "Windows PowerShell." 
 -  You may use the context menu to  pin it to the Start menu
    or the task bar. Then click the new icon that
    you placed on either Start menu or task bar
    to launch PowerShell. 
 -  If a PowerShell command fails and you are sure it is correct, close
    Powershell and re-launch wih the "Run as Administrator" option 
    (right-click).
 -  Learn the PowerShell commands to manage files and folders,
    including folders with spaces in the names (Tip: Quote folder names). 
    A good starting place is at
    [http://technet.microsoft.com/en-us/scriptcenter/dd772285.aspx](http://technet.microsoft.com/en-us/scriptcenter/dd772285.aspx).
    When practising with PowerShell, it is easiest at first to grasp
    what you are doing if you open Windows Explorer and PowerShell side by
    side and follow along in the graphical user interface.
    
##  About Macintosh Terminal 
  
