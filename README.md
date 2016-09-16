# resize_lvm_root

Ansible role for Extened LVM 

### Example

```
---
  - hosts: webservers
    vars:
      lv_name: 'lv_root'
      vg_name: 'VolGroup'
      vol_path:  '/dev/mapper/{{ vg_name }}-{{ lv_name }}'
      disk: '/dev/sda'
    roles:
      -  resize_lvm_root

```
