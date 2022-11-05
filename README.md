# vagrant-ubuntu

This is the base Ubuntu 22 box with a GUI enabled. I use it for testing the upgrade from Ubuntu 20 and for testing chezmoi for dotfiles management.

## Initialize

Initialize a new virtual machine from the Vagrantfile.

```bash
vagrant up
```

The terminal in which you run that command will show the initialization output

It may take a while because the `ubuntu-desktop` metapackage adds a lot of packages missing from the base box. 

VirtualBox will show a GUI whenever the virtual machine is running. Until initialization is complete, you can ignore it.

The virtual machine is rebooted at the end of the initialization to start the Ubuntu dekstop login experience. The VirtualBox GUI window will disappear during reboot and reappear.

At this point you can start working with Ubuntu via the GUI and follow the bootstrap steps in the chezmoi repo.

## Destroy

Clear it and start again.

```bash
vagrant destroy
```
