# qemu
A few qemu tools

## create-disk
Used to create the qcow2 OS disk.
```
./create-disk disk-name.qcow2 size-in-GB
```
Example:
```
./create-disk ubuntu.qcow2 20
```

## install
Install the OS to the disk - this may take awhile if KVM is not available!
```
./install disk-name.qcow2 iso-file [ -enable-kvm ]
```
Example:
```
./install ubuntu.qcow2 mini-ubuntu.iso [ -enable-kvm ]
```
Follow prompts to install.

## start
Run the VM
```
./start disk-name.qcow2
```
Example:
```
./start ubuntu.qcow2
```
