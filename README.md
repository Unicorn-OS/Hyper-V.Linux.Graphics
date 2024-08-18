# Hyper-V.Linux.Shared Graphics
https://www.google.com/search?q=hyper-v+ubuntu+graphics

discuss: https://superuser.com/questions/1660150/change-screen-resolution-of-ubuntu-vm-in-hyper-v

## Guide
https://gist.github.com/krzys-h/e2def49966aa42bbd3316dfb794f4d6a

```
$vm = "ubuntupv"

Set-VM -VMName $vm -GuestControlledCacheTypes $true -LowMemoryMappedIoSpace 1GB -HighMemoryMappedIoSpace 32GB
Add-VMGpuPartitionAdapter -VMName $vm
```
