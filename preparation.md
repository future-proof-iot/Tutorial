---
layout: default
title: Welcome to the IEEE EuroS&P RIOT Tutorial
---

# Preparatory Steps


We will use [RIOT](https://github.com/RIOT-OS/RIOT).
RIOT is an open source, real-time, multi-threading operating system
which supports a range of devices typically found in the Internet of Things,
based on various 32-bit, 16-bit or 8-bit microcontrollers.

For the tutorial we will use a preconfigured virtual
machine.
Please download and test-run the VM before the tutorial by following these [instructions & prerequisites](https://github.com/future-proof-iot/RIOT/wiki/SUIT-Tutorial-and-Hackathon-Berlin-2020).

### Manifest Generator

For the tutorial and hackathon, we will use the SUIT manifest generator. This can be [cloned from github](https://github.com/ARMmbed/suit-manifest-generator) and installed using pip, according to the installation [instructions](https://github.com/ARMmbed/suit-manifest-generator#installing). The SUIT manifest generator uses Python 3.6 or later.

### SUIT Manifest Parser Example

For the hackathon, there is a sample parser constructed in a bootloader. This is included in the SUIT Manifest Generator repository. This also requires srec_cat, arm-none-eabi-gcc, and mbed-cli. More detail and requirements are available in the [parser_examples](https://github.com/ARMmbed/suit-manifest-generator/tree/master/parser_examples) directory.

## TEEP

You can either use:

a. Visual Studio on an SGX-capable Windows laptop to code for SGX, or

b. Visual Studio Code on a Windows or Linux laptop to code for ARM TrustZone (for A class) or SGX.

### Visual Studio

The prerequisites are listed [here](https://github.com/dthaler/openenclave/blob/feature.vsextension/new_platforms/docs/VisualStudioWindows.md).  

#### SGX on Windows

To get the VS Extension in the fourth bullet, use the [HACKATHON private](
https://1drv.ms/u/s!Aqj-Bj9PNivcnu9xD1eiz0BAGLYlGw?e=kRKwDd) link there rather than the main VS marketplace link since v0.7 is not yet published in the marketplace.

If you need to know whether a machine is SGX1 or SGX1+FLC, you can get just the 'oesgx' tool for Linux and Windows [here](https://1drv.ms/u/s!Aqj-Bj9PNivcnu9uxhIkx-t_VYgHcw?e=bRAudK).

Walkthrough (not required before hackathon):

* See the Walkthrough section [here](https://github.com/dthaler/openenclave/blob/feature.vsextension/new_platforms/docs/VisualStudioWindows.md).

An OTrP prototype with TEEP stubs can be found here:

* GitHub repo: git clone --recursive https://github.com/dthaler/OTrP.git

#### SGX on Linux, using a Windows dev machine

The prerequisites are listed [here](https://github.com/dthaler/openenclave/blob/feature.vsextension/docs/GettingStartedDocs/VisualStudioLinux.md).  

### Visual Studio Code

Prerequisites:

* Install [Visual Studio Code](https://code.visualstudio.com/Download) (for Windows or Linux)

* Install the [Open Enclave extension](https://1drv.ms/u/s!Aqj-Bj9PNivcnu9t-U5vieHQZvzsog?e=3zp70h) private.
  (This update is not yet published in the VS Code marketplace.)

* Follow the other prerequisites listed [here](https://marketplace.visualstudio.com/items?itemName=ms-iot.msiot-vscode-openenclave#requirements)

Walkthrough (not required before hackathon):

* See the Getting Started section [here](https://marketplace.visualstudio.com/items?itemName=ms-iot.msiot-vscode-openenclave).
  If one runs VSCode and the extension on a Windows system, a Linux remote is necessary (WSL, VM, or physical).
