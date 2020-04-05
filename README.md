# Hack a Dell T3600 to work all devices using Mac Kexts
This is a simple script with default Dell T3600 Kexts to work all devices in Mac OS Sierra

### Backup current Kexts
First you need to copy all current Kexts with shell command like this

```
sudo -s
[enter password]
cp -r /System/Library/Extensions /System/Library/Extensions.backup
cp -r /mach_kernel /mach_kernel.backup
```

### Restore a new kexts

```
sudo -s
[enter password]
cp -r ./Extensions /System/Library/Extensions
```


### Rebuild Kexts Cache
After you copy all kexts to you operation system you need rebuild a kexts cache. Open your terminal and execute the command bellow using 
root user.

```
sudo kextcache -i /
```


### Download Kexts
[Download Kexts](http://drive.jaccon.com.br/s/S2RQ9Npnjoa9Kte) 
