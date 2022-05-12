# nodeOS

A random iso I made with nodejs as the userland.

## Running in QEMU

Assuming the iso is saved as nodeos.iso, to run it with qemu is just

```
qemu-system_x86_64 -cdrom nodeos.iso
```

## Bare metal

The iso has no efi suport, you will have to find a device supprort MBR booting.

You can make the iso bootable with a standard MBR with the isohybrid utility.

```
isohybrid nodeos.iso
```

Finaly you can flash it on to a usb, and boot!
