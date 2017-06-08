This file resolves a failure when creating a new VM from the "Install macOS 10.13 Beta.app"

The file "Create Mavericks Installer.tool" must replace the existing one located in: /Applications/VMware Fusion.app/Contents/Library/

Once replaced, Change the permissions of the file
```
sudo chmod 755 /Applications/VMware\ Fusion.app/Contents/Library/Create\ Mavericks\ Installer.tool
sudo xattr -rc /Applications/VMware\ Fusion.app/Contents/Library/Create\ Mavericks\ Installer.tool
```
You should be able to drag and drop the .app onto Fusion to begin the installation.

If you're still having problems a reboot sometimes helps.


There's more info on usage at our blog post [here](http://blogs.vmware.com/teamfusion/2016/06/fix-for-installing-macos-sierra-as-a-vm.html)
