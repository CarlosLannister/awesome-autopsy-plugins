# Awesome-Autopsy-Plugins [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
> A list of Autopsy awesome plugins.

:warning: = Autopsy Version >= 4.0 

## Plugins
- [Generic](#generic)
- [Windows](#windows)
- [Android](#android)
- [Law Enforcement](#lawenforcement)

### Generic 
### [Video Triage](http://www.autopsy.com/add-on-modules/autopsy-video-triage-module/)
> The Autopsy Video Triage module splits a video file into easily viewable thumbnail images (keyframes). By integrating directly in the Autopsy user interface, this module provides law enforcement, intelligence analysts, and investigators an efficient triage capability for video content.

### [Golden Image by Mathias Vetsch and Luca Taennler](https://github.com/colapse/Autopsy-GoldenImage)
> The Golden Image module uses two data sources – a “dirty image” and a “golden image” – and compares them with each other. The main task is, to find the difference between these two data sources – newly added files, deleted files and changed files.

### [Parse SQLite Del Rec by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Parse_SQLite_Del_Records)
> This module takes user input from a form. The user enters one or more SQLite database that they want to examine for deleted records into Autopsy. It will then export the specified SQLite database files to the temp directory then parse the SQLite database and create a custom artifact(s) for each table in the database. The custom artifacts have a name in the format of SQLite Database \<FileName\> Table \<Table Name\> DELETED Records with custom attributes for each artifact. Once it is complete the UI is notified that a new artifact has been added. This plugin can create a lot of extracted content so use it wisely. It is also not very fast on large database tables so this will need to be addressed in the future.

### [GoldBuild by John Lukach](https://github.com/jblukach/AutopsyModules/tree/master/GoldBuild)
> Export MD5 hashes to create a hash library for analysis

> Documentation - http://blog.4n6ir.com/2015/09/autopsy-python-gold-build-module.html

### [LowHangingFruit by John Lukach](https://github.com/jblukach/AutopsyModules/tree/master/LowHangingFruit)
> Export unknown hashes after analysis for Virus Total comparisons

> Documentation - http://blog.4n6ir.com/2015/09/autopsy-python-low-hanging-fruit-module.html

### [BuildMetaInfo by John Lukach](https://github.com/jblukach/AutopsyModules/tree/master/BuildMetaInfo)
> Export full path to SQLite database for meta data gold build

### [MatchMetaInfo by John Lukach](https://github.com/jblukach/AutopsyModules/tree/master/MatchMetaInfo)
> Compare meta data to identify unknown full paths hidden in plain sight

### [NetArchae by Emily Wicki](https://github.com/thePidge/netArchae)
> This Autopsy Module extracts Packet Captures (pcaps) from Data Sources. It then sorts them under a “PCAPs” tab within “Interesting Files” and allows the extracted pcaps to be parsed by KeywordSearch.

### [HashDump by John Lukach](https://github.com/jblukach/AutopsyMultiUserModules)
> HashDump.py creates a HashDump.txt file in the base of the case folder and it contains hashes of files in the case. HashDump was built as a proof of concept that requires the Hash Lookup Ingest Module be run prior to calculate the MD5 hashes. HashDump.py builds the ingest module for the Autopsy user interface that passes the case file location as an argument to the HashDump.exe python program.

> Documentation - http://blog.4n6ir.com/2016/05/autopsy-python-multi-user-modules.html

### [Parse SQLite DB by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Parse_SQLite_Databases)
> This module takes user input from a form. The user enters one or more SQLite database that they want to import into Autopsy. It will then export the specified SQLite database files to the temp directory then open the SQLite database and create a custom artifact(s) for each table in the database. The custom artifacts have a name in the format of SQLite Database \<FileName\> Table \<Table Name\> with custom attributes for each artifact. The blob database type is not handled and a text string message is specified stating this. Once it is complete the UI is notified that a new artifact has been added. This plugin can create a lot of extracted content so use it wisely. It is also not very fast on large database tables so this will need to be addressed in the future.
Payment Card Scanning Module  by Shea Nangle

### [Payment Card Scanning Module  by Shea Nangle](https://github.com/ultrashea/autopsy-payment-card-scanner)
> This Autopsy module will search for possible payment card numbers, and will then check the Luhn checksum of each possible payment card number, which will provide a greater degree of confidence regarding if a numeric sequence is a payment card number or not.

### [TagFilter by Mathias Vetsch and Luca Taennler](https://github.com/colapse/Autopsy-TagFilter)
> In Autopsy there are several tags of various modules which have the same or a similar meaning (For example tags to mark files as “known-good”). In Autopsy there is a listing of files per tag, but you might want to have a list containing all files that were tagged with “known-good”-a-like tags. The TagFilter module. This module enables you to create a list of files by applying several filters (for tags). You can add an unlimited amount of filters and connect them by AND-OR operators. Further on you can also specify f you want the filter to be true or false (File contains or doesn’t contain tag). Besides that, you can also create so called “Filter Groups” in which you can combine filters. The filters are applied top-down and they are built up similar to the SQL WHERE clause. You can also select if you want to search for files on all data sources within your case or just a specific one. In the end you will get a list with all the files that match your filter.

### [Virustotal online checker by Mathias Vetsch and Luca Taennler](https://github.com/mvetsch/VirusTotalOnlineChecker)
> Virustotal is an online service that allows to identify known-bad files. The service is free to use. The Virustotal online checker module allows to automatically check files on imported data sources against the virustotal service.

### Windows 
### [Prefetch Parser by Mark McKinnon](http://redwolfcomputerforensics.com/downloads/Autopsy_Python_Module_Process_Prefetch_Files.ziphttps://github.com/markmckinnon/Autopsy-Plugins/tree/master/Process_Prefetch_Files_V41)
> Parses prefetch on a windows computer and displays the details in the UI

### [FileMarker by John Lukach](https://github.com/jblukach/AutopsyModules/tree/master/FileMarker)
> Quick collection of important disk artifacts for triage
- File System: MFT, LogFile, UsnJrnl
- Event Logs: evtx
- pagefile.sys, hiberfil.sys and MEMORY.DMP
- Prefetch files: pf 
- SYSTEM, SECURITY, SOFTWARE, SAM, NTUSER.DATm, UsrClass.dat, RecentFileCache.bcf, Amcache.hve

> Documentation -  http://blog.4n6ir.com/2015/09/autopsy-python-file-marker-module.html 

### [Parse Amcache by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Process_Amcache)
> This module takes user input from a form. The user can select from three (3) Amcache reports to choose from, program entries, file entries and unassociated programs. It will then export the specified amcache.hve files to the temp directory then call an external program to parse out the programs and files and insert them into a SQLite database. The SQLite database is then imported into Autopsy and custom artifact(s) based on the user input will be created. The custom artifacts have a prefix of Amcache and custom attributes are created for each artifact. Once it is complete the UI is notified that a new artifact has been added.

### [ParseEvtx by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Process_EVTX)
> This module takes user input from a form. The user can select from three (3) default windows EVTX event logs or they can manually enter the logs they would like to parse. It will then export the specified EVTX files to the temp directory then call an external program to parse out the EVTX logs and insert them into a SQLite database. The SQLite database is then imported into Autopsy and a custom artifact named Windows Event Logs is created and custom attributes are created for this artifact. Once it is complete the UI is notified that a new artifact has been added. This works only on EVTX files.

### [Parse Plists by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Parse_Plist)
> This module takes user input from a form. The user enters one or more plist files that they want to export the information from. It will then export the specified Plist files to the temp directory then parse the Plist into a SQLite database and create a custom artifact(s) for each table in the database. The custom artifacts have a name in the format of Plist <FileName> with custom attributes for each artifact. Once it is complete the UI is notified that a new artifact has been added. This plugin can create a lot of extracted content so use it wisely. It is also not very fast on large Plist files so this will need to be addressed in the future.

### [SAMParse by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Parse_SAM)
> This module will extract the SAM registry files to the temp directory and then call an external program to parse the files and store the information into a SQLite database. The SQLite database will then be imported into a custom artifact named SAM File with custom attributes and will notify the UI after it is completed that a new artifact has been added to the Extracted content.

### [ShellBags by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Parse_Shellbags)
> This module will extract the each NTUSER.dat registry files to the temp directory and then call an external program to parse the shellbags for each user and store the information into a SQLite database. The SQLite database will then be imported into a custom artifact named Shellbags File with custom attributes and will notify the UI after it is completed that a new artifact has been added to the Extracted content.

### [ShimcacheParser by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Shimcache_parser)
> This module will extract the SYSTEM registry files to the temp directory and then call an external program to parse the Shimcache and store the information into a SQLite database. The SQLite database will then be imported into a custom artifact named Shimcache with custom attributes and will notify the UI after it is completed that a new artifact has been added to the Extracted content.

### [Parse SRUDB by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Process_SRUDB)
> This module takes user input from a form and based on the selection will import the System Resource Usage based on the user input. The module will then extract the SRUDB.DAT file to the temp directory and then call an external program to parse the SRUDB.dat file and store the information into a SQLite database. The SQLite database will then be imported into numerous custom artifact(s) based on what the user checks with custom attributes and will notify the UI after it is completed that a new artifact has been added to the Extracted content. This plugin may create numerous different artifacts.

### [USN Parser by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Parse_USNJ)
> This module will extract the $UsnJrnl:$J file to the temp directory and then call an external program to parse the Journal and store the information into a SQLite database. The SQLite database will then be imported into a custom artifact named NTFS UsrJrnl entries with custom attributes and will notify the UI after it is completed that a new artifact has been added to the Extracted content.

### [Parse WebCache by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Webcache)
> This module will extract all the WebcacheV01.dat files for all users to the temp directory and then call an external program to parse the Webcache and store the information into a SQLite database. The SQLite database will then be imported into numerous custom artifact(s) that have a prefix of Webcache in the name with custom attributes and will notify the UI after it is completed that a new artifact has been added to the Extracted content. This plugin may create numerous different artifacts.

### [JumpList AD by Mark McKinnon](https://github.com/markmckinnon/Autopsy-Plugins/tree/master/Jump_List_AD)
> This module will extract all the Jump list Auto destination files for all users to the temp directory and then call an external program to parse the files and store the information into a SQLite database. The SQLite database will then be imported into a custom artifact named Jump List Auto Dest with custom attributes and will notify the UI after it is completed that a new artifact has been added to the Extracted content.

### [P2P Forensic by Carlos Cilleruelo Rodríguez](https://github.com/CarlosLannister/P2PForensic)
> The main purpose of this plugin is try to get usage information of P2P Windows programs in a forensics environment. 

Supported P2P programs:
- Emule
- utorrent and BitTorrent

### [AuthentiCode Verification by Mathias Vetsch and Luca Taennler](https://github.com/mvetsch/Autopsy-AuthentiCodeVerification)
> The module verifies code signing certificates of Windows executables. It creates Content Tags with the Signer Name of the binary. This module helps to quickly eliminate known-good files from the OS vendor. You can also list the files from any unknown publisher, that signed software on the system you are investigating on. 

### Android 
### [Android Geodata XML/Crawler by Roberto Amelio](https://github.com/robiame/AndroidGeodata)
> The modules aim to collect and display significant amounts of data through which an investigator can consider reporting whereabouts the analysed mobile device has been taken.

### Law Enforcement
### [SmutDetect4Autopsy](https://github.com/rajwitt/SmutDetect4Autopsy)
> Simple Scan of JPG, BMP, PNG & GIF files (seletion of files based on file signatures) for pixels with skin tone and computing percentages. Files are tagged with skin-tone percentages in increments of 10 to allow a categorised view of thumbnails

> Documentantion - http://www.4ensics.co.uk/smutdetect4autopsy/

### [Project Vic and C4P/All integration](http://www.basistech.com/digital-forensics/autopsy/le-bundle/)
> Using these modules, you can automatically identify what images are known child exploitation images and get their categorization.

> Documentantion - http://www.basistech.com/digital-forensics/autopsy/le-bundle/
