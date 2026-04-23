Setting Up Windows VirtIO Drivers in Proxmox

Use the official VirtIO driver package for Windows guests in Proxmox:

https://fedorapeople.org/groups/virt/virtio-win/direct-downloads/archive-virtio/virtio-win-0.1.271-1/

Install the network driver in Windows
Open the Windows VM.
Go to Control Panel and open Device Manager.
Look for the Network Adapter with a yellow warning icon.
Right-click the device and choose Update Driver.
Select Browse my computer for drivers.

Navigate to the following folder on the VirtIO driver media:

netKVM\w10\amd64

Click Next or Confirm to install the driver.
Once installed, the warning icon should disappear and the network adapter should start working.
Notes
Make sure the VirtIO ISO or driver package is attached to the VM before starting.
The w10\amd64 path is for 64-bit Windows 10/11 guests.
