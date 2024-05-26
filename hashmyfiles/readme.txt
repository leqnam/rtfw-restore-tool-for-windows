


HashMyFiles v1.52
Copyright (c) 2007 - 2009 Nir Sofer
Web site: http://www.nirsoft.net



Description
===========

HashMyFiles is small utility that allows you to calculate the MD5 and
SHA1 hashes of one or more files in your system. You can easily copy the
MD5/SHA1 hashes list into the clipboard, or save them into text/html/xml
file.
HashMyFiles can also be launched from the context menu of Windows
Explorer, and display the MD5/SHA1 hashes of the selected file or folder.



System Requirements
===================

This utility works on Windows 2000/XP/2003/Vista/Windows 7. Older
versions of Windows are not supported.



Versions History
================


* Version 1.52:
  o Added sorting command-line options.

* Version 1.51:
  o Fixed bug: Modified Time and Created Time displayed the same
    date/time.

* Version 1.50:
  o Added 'Explorer Paste' option, which allows you to paste a list
    of files that copied from Explorer window or from any other software
    that copy files to the clipboard, including some utilities of
    NirSoft, like SearchMyFiles, IECacheView, and RegDllView. (by using
    the 'Explorer Copy' option)

* Version 1.47:
  o Fixed bug: Save command-line options failed to work in the last
    release.

* Version 1.46:
  o Fixed issue: When HashMyFiles window is hidden and there is an
    icon in the taskbar, running HashMyFiles again will open the existing
    instance of HashMyFiles, instead of creating another one.

* Version 1.45:
  o Added 'Put Icon In Tray' option.

* Version 1.43:
  o When you specify empty string ("") in the /folder command-line
    option, HashMyFiles will now use the current folder.

* Version 1.42:
  o Added AutoComplete to select folder dialog-box

* Version 1.41:
  o Fixed bug: 'Mark Hash In Clipboard' option marked all hashes when
    one or more hash types were deselected.

* Version 1.40:
  o Added 'Hash Types' sub-menu under options. Allows you to select
    which types of hashes you want to calculate.

* Version 1.37:
  o Fixed bug: When dragging a file into HashMyFiles window while
    it's already processed by HashMyFiles, the file was added multiple
    times.

* Version 1.36:
  o Fixed bug: When 'Add files in subfolders' was selected, only
    sub-folders files were added.

* Version 1.35:
  o Added 'Select Folder' dialog-box.
  o Added new option: 'Add files in subfolders'.
  o Added /folders command-line option
  o Added file extension column.
  o 'Select Process' dialog-box is now resizable.

* Version 1.31:
  o Added support for adding multiple files in 'Add File' option.

* Version 1.30:
  o Added new columns: File Version and Product Version. (for exe and
    dll files)

* Version 1.29:
  o Fixed bug: The main window lost the focus when the user switched
    to another application and then returned back to HashMyFiles.

* Version 1.28:
  o Display single file progress information (in percent) while
    hashing large files.

* Version 1.27:
  o Added new file type in save - comma-delimited file (.csv)
  o Added new command-line option - /scomma

* Version 1.26:
  o 'Mark Identical Hashes' option - now also works with saved HTML
    files and HTML reports.

* Version 1.25:
  o Add new column: 'Identical' - When there are 2 or more identical
    hashes, this column is filled with a number (1 for the first
    identical hashes, 2 for the second, and so on...)
  o Add 'Mark Identical Hashes' option - Mark identical hashes with
    up to 8 different colors.

* Version 1.20:
  o Fixed bug: When using 'Add Process Files' option, the filenames
    displayed in short path format.

* Version 1.19:
  o New command-line option: /files (support for loading multiple
    files)

* Version 1.18:
  o Fixed bug in Unicode version: wrong characters added to clipboard
    copy option.

* Version 1.17:
  o Added 'Mark Hash In Clipboard' option. If this options is
    selected, the hash that you copy to the clipboard is compared to the
    MD5/SHA1 hashes that are currently displayed in HashMyFiles. If there
    is a match, the hash line is marked in green color.

* Version 1.16:
  o Added 'FF FE' characters in the beginning of the saved Unicode
    files (Unicode version only).

* Version 1.15:
  o Fixed bug: HashMyFiles remained in memory if you closed it while
    calculating hashes.
  o New option: 'Add Process Files' - Allows you to get the hashes of
    all DLL files of the selected process.

* Version 1.10:
  o Explorer Context Menu - If an instance of HashMyFiles is already
    running, the selected files will be added to the existing instance,
    instead of creating a new one.
  o File icons are now displayed according to the file type.
  o New option: Always On Top.
  o Added 'Stop' menu item while calculating the hashes.
  o Added CRC32 calculations.
  o Added new columns: Modified Time, Created Time, and File Size.

* Version 1.00 - First Release.



Using HashMyFiles
=================

HashMyFiles doesn't require any installation process or additional DLL
files. In order to start using it, simply run the executable file
(HashMyFiles.exe).
After you run it, you can add files and folders that you want to view
their MD5/SHA1 hashes. You can do it by using the 'Add File' and 'Add
Folder' options under the File menu, or simply by draging the files and
folder from Explorer into the main window of HashMyFiles.
After adding the desired files, you can copy the MD5/SHA1 hashes to the
clipboard, or save the hashes list into text/html/xml file.



Explorer Context Menu
=====================

HashMyFiles can also be used directly from Windows Explorer. In order to
enable this feature, go to the Options menu, and choose the 'Enable
Explorer Context Menu' option. After you enable this feature, you can
right-click on any file or folder on Windows Explorer, and choose the
'HashMyFiles' item from the menu.
If you run the HashMyFiles option for a folder, it'll display the hashes
for all files in the selected folder.
If you run the HashMyFiles option for a single file, it'll display only
the hashes for that file.




Command-Line Options
====================



/file <Filename | Folder | Wildcard>
Specifies the filename, folder, or wildcard that you want to hash.

/files <Filename> <Filename> <Filename> ...
Specify multiple filenames, folders, or wildcards that you want to hash.

/folder <Folder>
Specify a folder and all its subfolders.

/stext <Filename>
Save the hashes list into a regular text file.

/stab <Filename>
Save the hashes list into a tab-delimited text file.

/stabular <Filename>
Save the hashes list into a tabular text file.

/shtml <Filename>
Save the hashes list into HTML file (Horizontal).

/sverhtml <Filename>
Save the hashes list into HTML file (Vertical).

/sxml <Filename>
Save the hashes list to XML file.

/scomma <Filename>
Save the hashes list to comma-delimited file.

/sort <column>
This command-line option can be used with other save options for sorting
by the desired column. If you don't specify this option, the list is
sorted according to the last sort that you made from the user interface.
The <column> parameter can specify the column index (0 for the first
column, 1 for the second column, and so on) or the name of the column,
like "Filename" and "Identical". You can specify the '~' prefix character
(e.g: "~Identical") if you want to sort in descending order. You can put
multiple /sort in the command-line if you want to sort by multiple
columns.



/nosort
When you specify this command-line option, the list will be saved without
any sorting.

Examples:
HashMyFiles.exe /file "c:\temp\*.zip" /shtml "c:\temp\1.html"
HashMyFiles.exe /file "d:\temp\myfile.zip" /stab "d:\temp\myfile.txt"
HashMyFiles.exe /file "d:\my files"
HashMyFiles.exe /files "c:\temp\*.zip" "c:\temp\1234.exe"
"c:\temp\Hello.exe" /shtml "c:\temp\1.html"
HashMyFiles.exe /folder "c:\temp" /shtml "c:\temp\1.html"
HashMyFiles.exe /folder "c:\temp" /shtml "c:\temp\1.html" /sort
"Identical" /sort "Filename"
HashMyFiles.exe /folder "c:\temp" /shtml "c:\temp\1.html" /sort ~1



Translating HashMyFiles to other languages
==========================================

In order to translate HashMyFiles to other language, follow the
instructions below:
1. Run HashMyFiles with /savelangfile parameter:
   HashMyFiles.exe /savelangfile
   A file named HashMyFiles_lng.ini will be created in the folder of
   HashMyFiles utility.
2. Open the created language file in Notepad or in any other text
   editor.
3. Translate all string entries to the desired language. Optionally,
   you can also add your name and/or a link to your Web site.
   (TranslatorName and TranslatorURL values) If you add this information,
   it'll be used in the 'About' window.
4. After you finish the translation, Run HashMyFiles, and all
   translated strings will be loaded from the language file.
   If you want to run HashMyFiles without the translation, simply rename
   the language file, or move it to another folder.



License
=======

This utility is released as freeware. You are allowed to freely
distribute this utility via floppy disk, CD-ROM, Internet, or in any
other way, as long as you don't charge anything for this. If you
distribute this utility, you must include all files in the distribution
package, without any modification !



Disclaimer
==========

The software is provided "AS IS" without any warranty, either expressed
or implied, including, but not limited to, the implied warranties of
merchantability and fitness for a particular purpose. The author will not
be liable for any special, incidental, consequential or indirect damages
due to loss of data or any other reason.



Feedback
========

If you have any problem, suggestion, comment, or you found a bug in my
utility, you can send a message to nirsofer@yahoo.com
