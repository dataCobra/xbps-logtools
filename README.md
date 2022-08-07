# System-Logging with /etc/logbook.txt

All changes to the system should be recorded in the /etc/logbook.txt file.
Changes that belong together are grouped together in a block that begins
with the date and the person who made the change. Within a block, the
actions are sorted chronologically, but newer blocks are inserted above
older ones.

By setting the LOGBOOK environment variable, a file other than
/etc/logbook.txt can be selected for the purpose of logging.

# Logbook maintenance tools

This script is used for semi-automatic maintenance of the logbook.
If no logbook exists, a new one will be created automatically.

logbook -- creates a new entry in the logbook.
Optionally, a text can be specified, which will be entered.

# XBPS specific commands
```
*  xbpsupg                 -- corresponds to 'xbps-install -Su' :
                              Updates all packages to the latests version.

*  xbpsins [PKG ...]       -- corresponds to 'xbps-install -S' :
                              Installs the specified packages from the repo.

*  xbpsrm [PKG ...]        -- corresponds to 'xbps-remove' :
                              Removes the specified packages.

*  xbpsrdp [PKG ...]       -- corresponds to 'xbps-remove -R'
                              Removes the specified packages and all the
                              dependencies that are no longer needed.

*  xbpsrop                 -- corresponds to 'xbps-remove -o'
                              Removes package orphans.
```
