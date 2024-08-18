# Hyper-V.Linux.Paravirt Graphics
This is based on WSLg but works for ordinary Hyper-V guest instances!

https://www.google.com/search?q=hyper-v+ubuntu+graphics

discuss: https://superuser.com/questions/1660150/change-screen-resolution-of-ubuntu-vm-in-hyper-v

## Guide
https://gist.github.com/krzys-h/e2def49966aa42bbd3316dfb794f4d6a

```
$vm = "ubuntupv"

Set-VM -VMName $vm -GuestControlledCacheTypes $true -LowMemoryMappedIoSpace 1GB -HighMemoryMappedIoSpace 32GB
Add-VMGpuPartitionAdapter -VMName $vm
```

# Source:
## oneclick-gpu-pv
>Enable GPU-PV easily
https://github.com/seflerZ/oneclick-gpu-pv

[VA-API video acceleration](https://github.com/seflerZ/oneclick-gpu-pv?tab=readme-ov-file#va-api-video-acceleration)

## Hyperv Linux Guest GPU PV
https://gist.github.com/OlfillasOdikno/f87a4444f00984625558dad053255ace
