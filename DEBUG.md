
MODEL=<path-to>/FVP-Base-RevC-2xAEMv8

KERNEL=../linux-linaro-stable/arch/arm64/boot/
DTB=xxx-t1.dtb

uart0.log:
```
## Flattened Device Tree blob at 82000000
   Booting using the fdt blob at 0x82000000
   Using Device Tree in place at 0000000082000000, end 0000000082005912

Starting kernel ...
```


KERNEL=~/Downloads/lt

uart0.log:
```
ERROR: Did not find a cmdline Flattened Device Tree
FDT and ATAGS support not compiled in - hanging
### ERROR ### Please RESET the board ###
```
