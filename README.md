# intel-igc
Linux 5.4 kernel driver for Intel(R) I225-LM/I225-V 2.5G Ethernet Controller

Current driver source is from the System76 build of [Linux 5.4.0-42](https://launchpad.net/~system76/+archive/ubuntu/proposed/+build/19851655).

Download the original kernel source using:

```
sudo apt source linux-image-5.4.0-7642-generic
```

## Installation

Install a dkms-based module from source with:

```
git clone https://github.com/jksinton/intel-igc.git
cd intel-igc

sudo ./install.sh

sudo rmmod igc
sudo modprobe igc
```

## Uninstall
Revert to the built in igc driver of the kernel
```
sudo ./uninstall.sh
sudo rmmod igc
sudo modprobe igc
```
