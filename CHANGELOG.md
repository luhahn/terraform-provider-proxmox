## 0.4.0 (UNRELEASED)

ENHANCEMENTS:

* resource/virtual_environment_vm: Add support for changing `disk.datastore_id` and `disk.size` without re-creating the VM

BUG FIXES:

* library/virtual_environment_nodes: Fix node IP address format

WORKAROUNDS:

* resource/virtual_environment_vm: Ignore default value for `cpu.architecture` when the root account is not being used

## 0.3.0

ENHANCEMENTS:

* resource/virtual_environment_container: Add `clone` argument
* resource/virtual_environment_container: Add `disk` argument
* resource/virtual_environment_container: Add `template` argument
* resource/virtual_environment_vm: Add `agent.timeout` argument
* resource/virtual_environment_vm: Add `audio_device` argument
* resource/virtual_environment_vm: Add `clone` argument
* resource/virtual_environment_vm: Add `initialization.datastore_id` argument
* resource/virtual_environment_vm: Add `serial_device` argument
* resource/virtual_environment_vm: Add `template` argument

BUG FIXES:

* resource/virtual_environment_container: Fix `network_interface` deletion issue
* resource/virtual_environment_vm: Fix `network_device` deletion issue
* resource/virtual_environment_vm: Fix slow refresh when VM is stopped and agent is enabled
* resource/virtual_environment_vm: Fix crash caused by assuming IP addresses are always reported by the QEMU agent
* resource/virtual_environment_vm: Fix timeout issue while waiting for IP addresses to be reported by the QEMU agent

OTHER:

* provider/docs: Add HTML documentation powered by GitHub Pages

## 0.2.0

BREAKING CHANGES:

* resource/virtual_environment_vm: Rename `cloud_init` argument to `initialization`
* resource/virtual_environment_vm: Rename `os_type` argument to `operating_system.type`

FEATURES:

* **New Data Source:** `proxmox_virtual_environment_dns`
* **New Data Source:** `proxmox_virtual_environment_hosts`
* **New Resource:** `proxmox_virtual_environment_certificate`
* **New Resource:** `proxmox_virtual_environment_container`
* **New Resource:** `proxmox_virtual_environment_dns`
* **New Resource:** `proxmox_virtual_environment_hosts`

ENHANCEMENTS:

* resource/virtual_environment_vm: Add `acpi` argument
* resource/virtual_environment_vm: Add `bios` argument
* resource/virtual_environment_vm: Add `cpu.architecture`, `cpu.flags`, `cpu.type` and `cpu.units` arguments
* resource/virtual_environment_vm: Add `tablet_device` argument
* resource/virtual_environment_vm: Add `vga` argument

## 0.1.0

FEATURES:

* **New Data Source:** `proxmox_virtual_environment_datastores`
* **New Data Source:** `proxmox_virtual_environment_group`
* **New Data Source:** `proxmox_virtual_environment_groups`
* **New Data Source:** `proxmox_virtual_environment_nodes`
* **New Data Source:** `proxmox_virtual_environment_pool`
* **New Data Source:** `proxmox_virtual_environment_pools`
* **New Data Source:** `proxmox_virtual_environment_role`
* **New Data Source:** `proxmox_virtual_environment_roles`
* **New Data Source:** `proxmox_virtual_environment_user`
* **New Data Source:** `proxmox_virtual_environment_users`
* **New Data Source:** `proxmox_virtual_environment_version`
* **New Resource:** `proxmox_virtual_environment_file`
* **New Resource:** `proxmox_virtual_environment_group`
* **New Resource:** `proxmox_virtual_environment_pool`
* **New Resource:** `proxmox_virtual_environment_role`
* **New Resource:** `proxmox_virtual_environment_user`
* **New Resource:** `proxmox_virtual_environment_vm`
