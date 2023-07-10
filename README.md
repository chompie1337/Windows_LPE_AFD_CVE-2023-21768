# CVE-2023-21768 Local Privilege Escalation POC

authors: [chompie](https://twitter.com/chompie1337) & [b33f](https://twitter.com/FuzzySec)

For demonstration purposes only. Complete exploit works on vulnerable Windows 11 22H2 systems. 
Write primitive works on all vulnerable systems.

Usage:

```
Windows_AFD_LPE_CVE-2023-21768.exe <pid>
```

where `<pid>` is the process ID (in decimal) of the process to elevate.

Should result in the target process being elevated to SYSTEM


The I/O Ring LPE primitive code is based on the I/ORing R/W [PoC](https://github.com/yardenshafir/IoRingReadWritePrimitive) by [Yarden Shafir](https://twitter.com/yarden_shafir)

Blog post [here](https://securityintelligence.com/posts/patch-tuesday-exploit-wednesday-pwning-windows-ancillary-function-driver-winsock/)