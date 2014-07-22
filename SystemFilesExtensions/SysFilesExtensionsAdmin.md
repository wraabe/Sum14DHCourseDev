
Some installation or update routines for open source software
require you to have an Administrator account or to run routines
in Administrator mode. 

If you do not have access to an Administrator account, you may
be denied permission to access certain files, install applications
or run applications. 

If your computer is infected with viruses or compromised, it is
more dangerous if the user accesses an administrator account. Therefore,
most software security and default setup includes an administrator account that is used
only occasionally, such as when installing software or performing
other processes that require Administrator rights.


## Administrator Account Passwords


To have an Administrator account on your computer, an account that has Administrator privileges must set up a new Admnistrator account or grant your current account Administrator privileges.

An administrator account should have a difficult password to crack. If you will use Administrator account only rarely, write it down on a slip of paper that you keep some place that is not be easily identifiable as the administrator account on your computer.

I recommend that you follow the recommendation of Neil O'Farrell, a computer security expert who advises that you create a password from a pnemonic version of a phrase, one constructed from a series of words that are meaningful to you and  from which you derive a long password with special characters,
   
   Phrase: "She dwelt among the untrodden ways."
   Password: sDaM_nguTdn*ys
   
The password advice is based on this post. (http://www.nealofarrell.com/20130829142/cybercrime/this-week-insecurity-august-29th-2013-is-it-truly-finally-sadly-game-over-for-passwords.html)[http://www.nealofarrell.com/20130829142/cybercrime/this-week-insecurity-august-29th-2013-is-it-truly-finally-sadly-game-over-for-passwords.html]


## Working in Administrator Mode

To have an Administrator account on your computer, an account that has Administrator privileges must set up a new Admnistrator account or grant your current account Administrator privileges.
   
For details on Administrator privileges on Macintosh OSX, see (http://support.apple.com/kb/PH10882?viewlocale=en\_US)[http://support.apple.com/kb/PH10882?viewlocale=en\_US].

For details on Administrator privileges on Windows OS, see (http://windows.microsoft.com/en-us/windows/change-users-account-type#1TC=windows-7)[http://windows.microsoft.com/en-us/windows/change-users-account-type#1TC=windows-7]

Remember, it is a security risk to work always in an Administrator account. Generally, it is better to complete a task that requires Administrator access and then return to your usual method. If you will work regularly in Administrator mode, you should have strong automatic backup routines as well as firewalls and virus protection.  
   

## Viewing File Extensions

The default (out of box) settings on many operating systems is to hide file extensions, the 3- or 4-character suffix to a file name that follows the period. The logic of that setting is that you associate files with individual applications or programs. This works reasonably well unless you are learning the command line or wishing to use more than one application for the same file. Because you will do both in this class, I recommend setting file extensions to be visible. 

For information on showing file extensions in Windows OS, see (http://windows.microsoft.com/en-us/windows/show-hide-file-name-extensions#show-hide-file-name-extensions=windows-7)[http://windows.microsoft.com/en-us/windows/show-hide-file-name-extensions#show-hide-file-name-extensions=windows-7]. 

For information on showing file extensions in Macintosh OSX, see (http://support.apple.com/kb/PH10845)[http://support.apple.com/kb/PH10845].


## Viewing Hidden System Files

Both Windows and Macintosh OS have a setting to make a file "Hidden," which helps prevent users from accessing application files and settings. Because you may need to view or alter settings files in Pandoc or LaTeX, which are kept in the applications directories, you may need to change settings temporarily so you can view hidden system files. 

Macintosh OS:

1.  Launch the Terminal and type the following command (Press "Enter" after the command):
~~~~
    defaults write com.apple.finder AppleShowAllFiles TRUE
~~~~ 

2.  Next step depends on your OS:

  *  In Lion or Mountain Lion, enter a second command on Terminal:
~~~~
    killAll Finder
~~~~ 

  * In Mavericks, Hold down `Alt` and click Finder in Dock for Mavericks.  Click Relaunch.

To reverse the setting (hide system files), type the following:

~~~~
    defaults write com.apple.finder AppleShowAllFiles FALSE
~~~~ 

*Note:* Frankly, this is very annoying in Mac OS. You may wish to search Google for add-ins that perform same task with GUI interface, like TinkerTool or Onyx. 

Windows OS:

For Windows, see the following guide:  (http://windows.microsoft.com/en-us/windows/show-hidden-files#show-hidden-files=windows-7)[http://windows.microsoft.com/en-us/windows/show-hidden-files#show-hidden-files=windows-7]

