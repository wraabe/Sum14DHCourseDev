## Introduction to Command Line Interfaces

Windows had two different command line interfaces, MS-DOS (command.exe or cmd.exe) and PowerShell (powershell.exe). MS-DOS ships with Windows, but PowerShell may need to be installed. On Macintosh computers, you will use the Terminal, the default UNIX shell. 

## About Windows Command Line Tools

Many PowerShell (Windows 7 and later) advantages over old MS-DOS Command Line concern networking and system administration, which you will not need in this course, but two important advantages of PowerShell are that it is more like UNIX command line and has an Administrator mode. On Windows 7 and later, MS-DOS command line may be denied access to system folders or commands. Many command line options that you are asked to perform  may also work on MS-DOS, but some will require PowerShell. 

## Note on Your Professor's Expertise

I am not an expert with either Windows PowerShell or the Macintosh Terminal for UNIX commands. I've been using Terminal several years, so I know a few commands. But I only use the tools when I need to, and turn to Internet searches when I need to learn unfamiliar command syntax. Working through a basic introductory tutorial will lower your rate of newby mistakes (which may save hours of frustration). But also turn back to instructions anytime that you have difficulty getting a command to work. These are essential tools for systems administrators and the like, but we will use them in this class only because some applications (like PanDoc) lack graphical user interfaces.

### Checking if PowerShell is installed

 - On the Start menu search box, type "PowerShell."
 - If not application is available, see "Installing Windows PowerShell"
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

 -  On the Start menu search box, type "Powershell," and right-click
    the "Windows PowerShell." 
 -  You may use the context menu to  pin it to the Start menu or the task bar. Then click the new icon that you placed on either Start menu or task bar to launch PowerShell. 
 -  If a PowerShell command fails and you are sure it is correct, close Powershell and re-launch wih the "Run as Administrator" option (right-click).
 -  Learn the PowerShell commands to manage files and folders,
    including folders with spaces in the names (Tip: Quote folder names with spaces). 
    
### Learning how to use PowerShell.   

 -  A good starting place is at [http://technet.microsoft.com/en-us/scriptcenter/dd772285.aspx](http://technet.microsoft.com/en-us/scriptcenter/dd772285.aspx).
 -  Review the tutorials on "Files and Folders," which should be enough for this course. But if you want to learn more advanced techniques, see tutorials on "Help and Information" and on "Saving and Importing."
 -  Note that the Windows folder "My Documents" may also be named plain "Documents" (no space) on the Command line. 
 -  Tip: When practising with PowerShell, it is easiest at first to grasp what you are doing if you open Windows Explorer and PowerShell side by side and follow along in the graphical user interface.
    
##  About Macintosh Terminal 
  
Modern Macintosh computers (beginning with OS X) are a UNIX-based operating system. When you launch the Terminal, you have access to full range of UNIX commands. Much online advice for open-access software presumes that you know how to access and use the command line and that you know UNIX commands also work in on Macintosh computers.  

### Running Macintosh Terminal

 1.  On the Spotlight (magnifying glass in upper right corner), search for "Terminal." Click the top entry to launch it.
 2.  To launch the terminal from the Dock (like other applications), return to Spotlight.  Click "Show All in Finder," Ctrl+click the top entry for "Terminal," select "Open Enclosing folder," and browse the /Applications/Utilities folder. After Terminal displays in list of utilities, you can drag a copy of the terminal icon down to the "Dock." From the Dock, click to launch the Terminal, which is a plain white box. 
3.   The default location for the file system to display is your Home location.
     
### Learning how to use the Terminal

  - A good place to start is the Apple Shell Scripting Primer at [https://developer.apple.com/library/mac/documentation/OpenSource/Conceptual/ShellScripting/Introduction/Introduction.html#//apple\_ref/doc/uid/TP40004268](https://developer.apple.com/library/mac/documentation/OpenSource/Conceptual/ShellScripting/Introduction/Introduction.html#//apple\_ref/doc/uid/TP40004268 ).
  -  In the Shell Scripting Primer, see "Appendix A."
  -  Tip: When practising with the Terminal, it may be easier at first to grasp what you are doing if you open the Finder and the Terminal side by side and follow along in the graphical user interface.
