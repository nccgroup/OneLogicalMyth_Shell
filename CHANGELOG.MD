# 29-10-2019 - Bug fixes, speed improvements and enhancements

Code tidy up using a ruler on 100 chars.

Replaced list domains with forest information button. This sees further infromation displayed including trust relationships.

LDAP query has been replaced with new LDAP query, this allows you to select the attributes returned. Results are now in a HTML table.

The read file button now displays the file within a <textarea> as some text was treated as HTML.

List drives now displays the drive type so you can identify any mapped network drives, any drives that can not be browsed are removed from the list to save errors.

Navigating a root of a drive now displays 'LIST DRIVES' instead of 'GO BACK ONE LEVEL'.

Local Users & Groups was running slow due to the way the object was called, now displays results instantly.

Other speed improvements have been introduced to reduce time to display results.

The `OneLogicalMyth.hta` has been renamed to `OneLogicalShell.hta` thanks to Nye (@nyep) for the suggestion. Repo name will stay the same to save confusion.
