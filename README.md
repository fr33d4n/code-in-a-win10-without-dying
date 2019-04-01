# Code in a win10 or die tryin
Just a bunch of files to make the process more bearable

## Included stuff:
- Vagrantfile with some basic stuff (latest ubuntu, git, essentials, nvm). To create a fresh VM and start coding: 
  - Install Virtualbox and Vagrant from them respective internet sites. 
  - Create a folder which will store your VM
  - Customize the Vagrantfile. Its necessary to, at least change the windows folder(s) that will be shared between W10 and the VM. 
  - Go to the Folder previously created and run `vagrant up`
  - Once the VM has been created you can enter it with `vagrant ssh`

- VSCode OSX rebinds, AKA, how not to hate your life if you've beed developing on Mac for +5 years and now you're stuck with another sub silicon form. To install it: 
  - Open the VSCode terminal (shift + ctrl + P)
  - search for keybind
  - copypaste the vsCode rebinds (JSON) there. You must open the JSON file, not the interactive one.

- .bashrc with some really usefull stuff (Git helpers, nvm helpers)
- Mandatory: Enable windows symlinks (https://superuser.com/questions/124679/how-do-i-create-a-link-in-windows-7-home-premium-as-a-regular-user?answertab=votes#125981): 
  - Right click on Start→Run and launch secpol.msc.
  - Open Security Settings → Local Policies → User Rights Assignment and select Create symbolic links (that represents SeCreateSymbolicLinkPrivilege).