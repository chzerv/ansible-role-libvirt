# Ansible Role: Libvirt

This role installs and configures `libvirt` on Debian-based, RedHat-based and Archlinux systems.

## Requirements

None.

## Role Variables

`libvirt_selinux_booleans`

> SELinux booleans to be applied. Make sure to read [RedHat's documentation](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/8/html-single/configuring_and_managing_virtualization/index#virtualization-booleans-in-rhel-8_securing-virtual-machines-in-rhel-8) on securing VMs. 

` libvirt_install_virt_manager: true`

> Whether to install virt-manager or not. Virt-manager is a GUI front-end for libvirt, so it is most likely
> useless in headless systems.

`libvirt_uefi_vm_support: true`

> Install OVMF packages which provide the ability to create VMs using UEFI boot mode.

`libvirt_access_vms_using_hostnames: true`

> Enable the `libvirt` NSS module which allows host access to guests on non-isolated networks.

`libvirt_users_in_libvirt_group: []`

> A list of users that will be added to the `libvirt` group. Users of this group are allowed password-less access
> to the libvirt daemon.

## Dependencies

None.

## Example Playbook

WIP.

## License

MIT / BSD

## Author Information

Xristos Zervakis
