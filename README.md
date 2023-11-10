# Ansible Machine

This project first used Vagrant to create a base Debian libvirt virtual machine.
It then uses Ansible to setup the machine.

## Create Initial Machine
```
vagrant up
```

## Destroy Machine
```
vagrant destroy -f
```

## SSH In
While creating the machine, a ssh key will be generated for a `vagrant` user.
To login with this key, just enter:
```
vagrant ssh
```

## After Vagrant Up

### Set Pauls password
To login as `paul` in Gnome, the user will need a password.  Set it by ssh'ing as vagrant
and setting it with:
```
vagrant ssh
> sudo passwd paul
```

### Install Neovim Packer
To Neovim running, open it up with `nvim`, then hit `q` until the error messages calm down. 
Then run `PackerSync`.  On restart, NeoVim should look cool.

### Tmux Plugins
To install the tmux plugins, run `tmux` then type `<C-a> + I`.
This will run TPM and download the plugins.

### Screen Resolution
For now, just head to Gnome Display settings to adjust the resolution.



