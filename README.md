# Setting Up Windows VirtIO Drivers in Proxmox

Use the official VirtIO driver package for Windows guests in Proxmox:

[VirtIO Windows Drivers](https://fedorapeople.org/groups/virt/virtio-win/direct-downloads/archive-virtio/virtio-win-0.1.271-1/)

## Install the Network Driver in Windows

1. Open the Windows VM.
2. Go to **Control Panel** and open **Device Manager**.
3. Find the **Network Adapter** with a yellow warning icon.
4. Right-click the device and select **Update Driver**.
5. Choose **Browse my computer for drivers**.
6. Browse to this folder on the VirtIO driver media:

   `netKVM\w10\amd64`

7. Click **Next** to install the driver.
8. After installation, the warning icon should disappear and the network adapter should begin working.

## Notes

- Make sure the VirtIO ISO or driver package is attached to the VM before booting.
- The `w10\amd64` path is for **64-bit Windows 10 and Windows 11** guests.
