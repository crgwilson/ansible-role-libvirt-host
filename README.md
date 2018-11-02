# Role: Libvirt-host

Perform some basic bootstrapping for a [KVM hypervisor](https://wiki.debian.org/KVM#Installation).

## Whats it do?

- Install packages necessary for a libvirt server
- Configure a virtual bridge interface (to be used by created VMs) in the hackiest way possible

## But why?

This role is meant for some quick and dirty bootstrapping of my lab. Everything is
pretty hardcoded to that end at the moment and it will be difficult to try and
use this for anything else.

## OS Compatibility

- Debian 9 (stretch)

### Note:

Theoretically this should also work on older versions of Debian as well, but I have
not actually tested it.

