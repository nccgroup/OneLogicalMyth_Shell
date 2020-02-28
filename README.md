# OneLogicalMyth_Shell

This HTA shell was created to assist in breakout assessments. I built this over a year ago initally and thought others might find it useful so have now made it public. Please feel free to submit pull requests.

# Features
## File Explorer
* List Drives - Lists all local drives on the host. You can then click a drive letter to start navigating folders and files.
* List Folder - Entering a folder path in the top input box and clicking this button will start navigation at this point.
* User Profile Folder - Starts navigation at the `%userprofile%` folder.
* Read File - Entering a file path in the top input box and clicking this button will display the file contents in the window. For images these are displayed as images instead.
* Get DACL - Displays the NTFS permissions for a file or folder.
## System Info
* Local Users & Groups - Enumerates all groups and their memberships.
* Scheduled Tasks - Produces a highlevel task list in an HTML table, this can be copied into Excel for filtering for example.
* Local Password Policy - Runs `net accounts` and displays output within the window.
## Active Directory
* Forest Information - Lists information about the local computers forest if domain joined including trust relationships.
* New LDAP Query - Displays a form to run an LDAP query. The attributes selected are then presented in a HTML table.
## Data Upload/Download
HTTP File Download - Downloads a file to the file path provided. If the file exists will prompt to overwrite.
HTTP File Upload - Uploads a file using a POST request. This has been tested with Droopy.
## Other
* Run Program (Interactive) - Runs the specified command in the input box and interactively displays it. Useful for launching `powershell.exe` etc. Does not bypass restrictions.
* Run Program (Background) - Runs the specified command in the input box and captures the standrd out to the window. Useful for running comands that close on exit. Does not bypass restrictions.
* Run XML for MSBuild - Using the specified XML file in the input box this is run against MSBuild.exe.
