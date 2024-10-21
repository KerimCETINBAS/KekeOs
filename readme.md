### KekeOs (son derece işleviz işletim sistemi)



### build 

make sure have docker installed on your system

```bash
docker build buildenv -t kekeos-buildenv        
```


connect container with interactive terminal
```
 docker run --rm -it -v .:/root/env kekeos-buildenv   
```

on container's terminal
```bash
make build-x86_64
```

### usage

you can try with an emulator
https://www.qemu.org/


```bash
 qemu-system-x86_64 -cdrom dist/x86_64/karnel.iso
```