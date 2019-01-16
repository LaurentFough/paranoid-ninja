# paranoid-ninja

# about 

A script to protect your privacy and your system :).  
Randomize MAC address, localtime, private ip, transparent-torrify with nftables (for now) and patch the kernel with harden feature recommanded by [ClipOS](https://docs.clip-os.org/clipos/kernel.html) and [KernSec](https://kernsec.org/wiki/index.php/Kernel_Self_Protection_Project/Recommended_Settings).

## Dependencies

iproute2, shuf, urandom, util-linux, nftables, systemd.

### Kernel
Combine the configuration of [ClipOS](https://docs.clip-os.org/clipos/kernel.html) and [KernSec](https://kernsec.org/wiki/index.php/Kernel_Self_Protection_Project/Recommended_Settings).  
**TODO List** 
+ Add compilation for systemd
+ Add compilation for iptables
+ Add kernel boot params for grub2

### Firewall
Just add a basic and secure firewall with log and transparent proxy with TOR, inspired by the script [kalitorify](https://github.com/brainfucksec/kalitorify.git), i've create custom rule for nftables.  
**TODO List** 
+ add iptables rules.

### Systemd
I'll write some services especially for randomize the MAC address,the timezone and the hostname at boot.  
**TODO List**
+ randomize localtime

Be careful, the project is not ready for production :)

## Install

    # git clone https://github.com/szorfein/paranoid-ninja.git

## Usage

    # ./paranoid.sh -h

