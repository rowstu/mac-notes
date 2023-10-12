# Terminal Commands

Flush DNS
```
sudo dscacheutil -flushcache; sudo killall -HUP mDNSResponder
```
Open the print queue (via system settings) when you receive this sill error: "<strong>You must be an administrator to delete this job.</strong>":
```
sudo open "x-apple.systempreferences:com.apple.preference.security"
```
all print jobs can also be cancelled with the following command:
```
cancel -a -x
```
Run a system update:
```
softwareupdate -i -a
```
Increase the space between items in the Dock:
```
defaults write com.apple.dock persistent-apps -array-add '{"tile-type"="spacer-tile";}'; killall Dock
```
Show hidden files in the Finder:
```
defaults write com.apple.finder AppleShowAllFiles TRUE; killall Finder
```
Hide hidden files:
```
defaults write com.apple.finder AppleShowAllFiles FALSE; killall Finder
```
Rename the machine and Bonjour name:
```
sudo scutil –set ComputerName <newComputerName>
sudo scutil –set LocalHostName <newBonjourName>
```
Domain join the machine:
```
sudo dsconfigad -preferred <adserver.example.com> -a <computername> –domain example.com -u administrator -p <password>
```
Clear RAM:
```
purge
```
Create a password protected zip
```
zip -e protected.zip /path/name
```
