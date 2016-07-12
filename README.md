This file resolves a failure when creating a new VM from the "Install 10.12 Developer Preview.app" 

The file "Create Mavericks Installer.tool" must replace the existing one located in: /Applications/VMware Fusion.app/Contents/Library/

Once replaced, Change the permissions of the file
```
sudo chmod 755 /Applications/VMware\ Fusion.app/Contents/Library/Create\ Mavericks\ Installer.tool
sudo xattr -rc /Applications/VMware\ Fusion.app/Contents/Library/Create\ Mavericks\ Installer.tool
```
You should be able to drag and drop the .app onto Fusion to begin the installation.

If you're still having problems a reboot sometimes helps.


