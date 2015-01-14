# Administrator Accounts and Security, File Extensions, and Hidden System Files 

The default settings on modern operating systems (Windows 7 and 8, Mac OSX) shield users from some rather rudimentary geekery in order to present users with a graphical user interface. To work with open-source and non-commercial software, you may need to review the wizardry behind the curtain. Three basic steps are to run routines with an Administrator account, to view file extensions, and to view hidden files. 

Getting access to these advanced tools is not risk-free: the designers of operating systems hid them from you on the assumption that everyday users are safer users if they cannot see behind the scenes. But the risk is comparatively low. Nonetheless, if your computer is infected with viruses or compromised, it is more dangerous if the virus or other form of compromise has access to an administrator account. Therefore, most software security and default setup includes an administrator account that is used only occasionally, such as when installing software or performing other processes that require Administrator rights. 

Therefore, I do recommend that you step up your security routines for passwords when you start modifying these more advanced features.

## Administrator Account Passwords

To have an Administrator account on your computer, an account that has Administrator privileges must set up a new Administrator account or grant your current account Administrator privileges.

An administrator account should have a difficult password to crack. If you will use Administrator account only rarely, write it down on a slip of paper that you keep some place that is not be easily identifiable as the administrator account on your computer.

Neil O'Farrell is a computer security expert who advises that you create a password from a mnemonic version of a phrase, one constructed from a series of words that are meaningful to you and  from which you derive a long password with special characters:

From this phrase: “She dwelt among the untrodden ways.” 
This password: `sDaM_nguTdn*ys`
Or this one: `SDAT*ntr10*ys`

For more on O'Farrell's password advice, see &lt;[http://www.nealofarrell.com/20130829142/cybercrime/this-week-insecurity-august-29th-2013-is-it-truly-finally-sadly-game-over-for-passwords.html](http://www.nealofarrell.com/20130829142/cybercrime/this-week-insecurity-august-29th-2013-is-it-truly-finally-sadly-game-over-for-passwords.html)&gt;. This method is not uncrackable, but you can be reasonably certain that your password won't be guessed by someone who tries one of the 300 or 500 or 5,000 most common passwords.

## Administrator Mode and Security Software

### Administrator Mode

To have an Administrator account on your computer, an account that has Administrator privileges must set up a new Administrator account or grant your current account Administrator privileges.

For details on Administrator privileges on Macintosh OSX, see &lt;[http://support.apple.com/kb/PH10882?viewlocale=en\_US](http://support.apple.com/kb/PH10882?viewlocale=en\_US)&gt;.

For details on Administrator privileges on Windows OS, see &lt;[http://windows.microsoft.com/en-us/windows/change-users-account-type#1TC=windows-7](http://windows.microsoft.com/en-us/windows/change-users-account-type#1TC=windows-7)&gt;

It is a security risk to work always in an Administrator account. Generally, it is better to complete a task that requires Administrator access and then return to a power user account. If you will work regularly in Administrator mode, you should have strong automatic backup routines and use both a firewall and virus protection. 

### Essential Security Software

Kent State provides free downloads of Microsoft Security Essentials (Windows) and Sophos Anti-Virus (Mac). You should install the appropriate ones for your operating system and set them to update automatically. See &lt;[http://bbcrm.edusupportcenter.com/link/portal/8096/8210/Article/9702/Where-can-I-find-Kent-State-software-downloads#Mac4All](http://bbcrm.edusupportcenter.com/link/portal/8096/8210/Article/9702/Where-can-I-find-Kent-State-software-downloads#Mac4All)&gt;

## Viewing File Extensions

The default (out of box) settings on many operating systems is to hide file extensions, the 3- or 4-character suffix to a file name that follows the period. The logic of that setting is that you associate files with individual applications or programs. This works reasonably well unless you are learning the command line or wishing to use more than one application for the same file. Because you will do both in this class, I recommend setting file extensions to be visible. 

For more information on showing file extensions in Windows OS, see &lt;[http://windows.microsoft.com/en-us/windows/show-hide-file-name-extensions#show-hide-file-name-extensions=windows-7](http://windows.microsoft.com/en-us/windows/show-hide-file-name-extensions#show-hide-file-name-extensions=windows-7)&gt;. 

For more information on showing file extensions in Macintosh OSX, see &lt;[http://support.apple.com/kb/PH10845](http://support.apple.com/kb/PH10845)&gt;.

## Viewing Hidden System Files

Both Windows and Macintosh OS have a setting that automatically sets some file attributes to “Hidden,” which prevents unwitting users from accessing application files and settings. Because you may need to view or alter settings files in Pandoc or LaTeX, which are typically installed to application directories (although Windows users are advised to install LaTeX to the C directory), you may need to change settings temporarily so that you can view hidden system files. 

### Macintosh OS:

1.  Launch the Terminal and type the following command on one line (Press “Enter" after the command):
~~~~
    defaults write com.apple.finder AppleShowAllFiles TRUE
~~~~ 

2.  Next step depends on your OS:

  *  In Lion or Mountain Lion, enter a second command on Terminal:
~~~~
    killAll Finder
~~~~ 

  * In Mavericks, hold down `Alt` key, and click Finder in Dock for Mavericks.  Click Relaunch.

To reverse the setting (hide system files), type the following:

~~~~
    defaults write com.apple.finder AppleShowAllFiles FALSE
~~~~ 

 > *Note:* The command-line procedures in Mac OS can move quickly to UNIX geekery. Search Google or App Store for add-ins that perform same task with GUI interface. Two such tools are TinkerTool and Onyx. 

### Windows OS:

For Windows, see the following guide:  &lt;[http://windows.microsoft.com/en-us/windows/show-hidden-files#show-hidden-files=windows-7](http://windows.microsoft.com/en-us/windows/show-hidden-files#show-hidden-files=windows-7)&gt;

