# Linux_on_FVP_Base_Revc_2xAEMvA
run linux on FVP, 


## Download FVP first
This repo stick to the FVP_Base_RevC
```
wget https://developer.arm.com/-/media/Files/downloads/ecosystem-models/FVP_Base_RevC-2xAEMvA_11.17_21.tgz
```

## Quickstart

build
```
mkdir workspace

# packed script
unzip fvp-latest-oe-uboot.zip -d ./workspace

# FVP
tar -xvf FVP_Base_RevC-2xAEMvA_11.17_21.tgz -C workspace

# disk
wget https://releases.linaro.org/archive/15.05/openembedded/aarch64/vexpress64-openembedded_minimal-armv8-gcc-4.9_20150522-720.img.gz
tar -xvf vexpress64-openembedded_minimal-armv8-gcc-4.9_20150522-720.img.gz > ./workspace/vexpress.img
```

run
```
cd workspace
export DISK=./vexpress.img
export MODEL=./Base_RevC_AEMvA_pkg/models/Linux64_GCC-9.3/FVP_Base_RevC-2xAEMvA
./run_model.sh
```


## build from raw
1. FVP Model
2. Linux Image
3. rootfs/ disk image
4. boot loader image 


### FVP
Fixed Virtual Platforms (FVP) for development of software for Armv8-A and Armv8-M. The platform includes the Architecture Envelope Model (AEM) for Armv8 and a comprehensive set of SystemIP. The FVPs are updated quarterly and model the latest published architecture specifications.
```
wget https://developer.arm.com/-/media/Files/downloads/ecosystem-models/FVP_Base_RevC-2xAEMvA_11.17_21.tgz
```


### Linux Image
- linaro


### rootfs/ disk image
- buildroot: a simple, efficient and easy-to-use tool to generate embedded Linux systems through cross-compilation.
- get from 

###

