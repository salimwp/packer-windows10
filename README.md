# packer-Windows10

This repo contains the files needed to create a virtualbox image of Windows 10. Please download the Windows 10 ISO from Microsoft's website and make the necessary changes to the Windows10.json file.

Once the changes have been made run the following command:

```sh
$ packer build Windows10.json
virtualbox-iso: output will be in this color.

==> virtualbox-iso: Retrieving Guest additions
==> virtualbox-iso: Trying /usr/share/virtualbox/VBoxGuestAdditions.iso
==> virtualbox-iso: Trying /usr/share/virtualbox/VBoxGuestAdditions.iso
==> virtualbox-iso: /usr/share/virtualbox/VBoxGuestAdditions.iso => /usr/share/virtualbox/VBoxGuestAdditions.iso
==> virtualbox-iso: Retrieving ISO
```

The process is rather long, approx 30 minutes. The import appliance feature for Virtual Box doesn't work so create a new VM and mount the VMDK volume to the VM.
