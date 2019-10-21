# OneLogicalMyth_Shell

This HTA shell was created to assist in breakout assessments. I built this over a year ago initally and thought others might find it useful.

# Features
## File Explorer
* List Drives - Lists all local drives on the host. You can then click a drive letter to start navigating folders and files.
* List Folder - Entering a folder path in the top input box and clicking this button will start navigation at this point.
* User Profile Folder - Starts navigation at the `%userprofile%` folder.
* Read File - Entering a file path in the top input box and clicking this button will display the file contents in the window. For images these are displayed as images instead.
## System Info
* Local Users & Groups - Enumerates all groups and their memberships.
* Scheduled Tasks - Produces a highlevel task list in an HTML table, this can be copied into Excel for filtering for example.
* Local Password Policy - Runs `net accounts` and displays output within the window.
## Active Directory
* List Domains - Lists all domains identified within the local computers forest if domain joined. Local forest only, excludes trusts.
* Run LDAP Query - Runs an LDAP query using the LDAP filter specified in the input box. Currently only `sAMAccountName` and `distinguishedName` are returned.
## Other
* Run Program (Interactive) - Runs the specified command in the input box and interactively displays it. Useful for launching `powershell.exe` etc. Does not bypass restrictions.
* Run Program (Background) - Runs the specified command in the input box and captures the standrd out to the window. Useful for running comands that close on exit. Does not bypass restrictions.
* Run XML for MSBuild - Using the specified XML file in the input box this is run against MSBuild.exe.
