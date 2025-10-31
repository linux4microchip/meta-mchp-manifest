# Microchip Yocto Project Manifests

This repository provides manifests to build the [Microchip Yocto Project BSP](https://github.com/linux4microchip/meta-mchp).

## Install the repo utility

To use the manifests within this repository, the `repo` tool must be installed first.

```bash
$ mkdir ~/bin
$ curl http://commondatastorage.googleapis.com/git-repo-downloads/repo  > ~/bin/repo
$ chmod a+x ~/bin/repo
$ PATH=${PATH}:~/bin
```

## Download the Microchip PolarFire SoC Manifest

```bash
$ mkdir yocto-dev && cd yocto-dev
$ repo init -u https://github.com/linux4microchip/meta-mchp-manifest.git -b refs/tags/linux4microchip+fpga-2025.10 -m polarfire-soc/default.xml
$ repo sync
```

## Download the MPU SoC Manifest

```bash
$ mkdir yocto-dev && cd yocto-dev
$ repo init -u https://github.com/linux4microchip/meta-mchp-manifest.git -b refs/tags/linux4microchip-2025.04 -m mpu/default.xml
$ repo sync
```

## Download the PIC64GX Manifest

```bash
$ mkdir yocto-dev && cd yocto-dev
$ repo init -u https://github.com/linux4microchip/meta-mchp-manifest.git -b refs/tags/linux4microchip+fpga-2025.10 -m pic64/pic64gx/default.xml
$ repo sync
```

For instructions on how to setup and build the Microchip Yocto BSP please refer to the [Microchip Yocto BSP README](https://github.com/linux4microchip/meta-mchp/blob/scarthgap/meta-mchp-common/README.md).
