# Pix4Dmapper Ansible role

This Ansible role installs Pix4D Mapper

[Pix4Dmapper](https://pix4d.com/product/pix4dmapper/) is a photogrammetry software for professional drone-based mapping.


## Requirements

Currently only deb package is availa

It’s a comercial software and requires a licence you can [get here](https://cloud.pix4d.com/store/?=&solution=pro#solution_pro)


## Instalation

`ansible-galaxy install luisffc.pix4dmapper`


## Role Variables

Available variables are listed below, along with default values:

`pix4dmapper_version: 3.3.29`


## Example Playbook

- Using default version

```
    - hosts: servers
      roles:
         - luisffc.pix4dmapper
```


- Using a different version

```
    - hosts: servers
      roles:
         - { role: luisffc.pix4dmapper, pix4d_version: "3.3.29" }
```
