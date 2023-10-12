# Terminal Commands

Flush DNS
```
sudo dscacheutil -flushcache; sudo killall -HUP mDNSResponder
```

Open the print queue (via system settings) when you receive this sill error: "<strong>You must be an administrator to delete this job.</strong>"
```
sudo open "x-apple.systempreferences:com.apple.preference.security"
```
all print jobs can also be cancelled with the following command:
```
cancel -a -x
```
