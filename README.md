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
$ repo init -u https://github.com/linux4microchip/meta-mchp-manifest.git -b scarthgap -m polarfire-soc/default.xml
```

For instructions on how to setup and build the Microchip Yocto BSP please refer to the [Microchip Yocto BSP README](https://github.com/linux4microchip/meta-mchp/meta-mchp-common/README.md).
