# Ansible collection: kangaroot.foreman_content_redhat

Collection for configuring Red Hat repositories and Red Hat OS related content in a Foreman/Katello installation.

The Red Hat repositories that can be configured from this collection are:

Red Hat standard repositories:

- Red Hat Enterprise Linux Server 7 Server x86_64:
  - Red Hat Enterprise Linux 7 Server
  - Red Hat Enterprise Linux 7 Server - Extras
  - Red Hat Enterprise Linux 7 Server - Optional
  - Red Hat Enterprise Linux 7 Server - Supplementary
  - Red Hat Enterprise Linux 7 Server - Fastrack
  - Red Hat Enterprise Linux 7 Server - Optional Fastrack
  - Red Hat Enterprise Linux 7 Server - RH Common
  - Red Hat Satellite Client 6 for RHEL 7 Server
  - Red Hat Satellite 6 Client 2 for RHEL 7 Server
  - Red Hat Satellite Maintenance 6 for RHEL 7 Server
  - Red Hat Satellite Maintenance 6.11 for RHEL 7 Server
  - Red Hat Satellite Tools 6.10 for RHEL 7 Server
  - Red Hat Satellite Utils 6.11 for RHEL 7 Server
  - Red Hat Software Collections RPMs for Red Hat Enterprise Linux 7 Server
  - Red Hat Ansible Engine 2 RPMs for Red Hat Enterprise Linux 7 Server
  - Red Hat Ansible Engine 2.9 RPMs for Red Hat Enterprise Linux 7 Server

- Red Hat Enterprise Linux for x86_64 8[^1]:
  - Red Hat Enterprise Linux 8 for x86_64 - BaseOS
  - Red Hat Enterprise Linux 8 for x86_64 - AppStream
  - Red Hat Enterprise Linux 8 for x86_64 - Supplementary
  - Red Hat Satellite Client 6 for RHEL 8 x86_64
  - Red Hat Satellite 6 Client 2 for RHEL 8 x86_64
  - Red Hat Satellite Tools 6.10 for RHEL 8 x86_64
  - Red Hat Satellite Utils 6.11 for RHEL 8 x86_64
  - Red Hat Satellite Utils 6.12 for RHEL 8 x86_64
  - Red Hat Satellite Utils 6.13 for RHEL 8 x86_64
  - Red Hat Satellite Utils 6.14 for RHEL 8 x86_64
  - Red Hat Satellite Utils 6.15 for RHEL 8 x86_64
  - Red Hat Satellite Utils 6.16 for RHEL 8 x86_64
  - Red Hat Satellite Maintenance 6.11 for RHEL 8 x86_64
  - Red Hat Satellite Maintenance 6.12 for RHEL 8 x86_64
  - Red Hat Satellite Maintenance 6.13 for RHEL 8 x86_64
  - Red Hat Satellite Maintenance 6.14 for RHEL 8 x86_64
  - Red Hat Satellite Maintenance 6.15 for RHEL 8 x86_64
  - Red Hat Satellite Maintenance 6.16 for RHEL 8 x86_64
  - Red Hat Ansible Engine 2 for RHEL 8 x86_64
  - Red Hat Ansible Engine 2.9 for RHEL 8 x86_64

- Red Hat Enterprise Linux for x86_64 9[^1]:
  - Red Hat Enterprise Linux 9 for x86_64 - BaseOS
  - Red Hat Enterprise Linux 9 for x86_64 - AppStream
  - Red Hat Enterprise Linux 9 for x86_64 - Supplementary
  - Red Hat Satellite Client 6 for RHEL 9 x86_64
  - Red Hat Satellite 6 Client 2 for RHEL 9 x86_64
  - Red Hat Satellite Utils 6.16 for RHEL 9 x86_64
  - Red Hat Satellite Maintenance 6.16 for RHEL 9 x86_64

Red Hat kickstart respositories:

- Red Hat Enterprise Linux Server 7 (x86_64) kickstart[^2]
- Red Hat Enterprise Linux for x86_64 8 kickstart[^2]: BaseOS / AppStream
- Red Hat Enterprise Linux for x86_64 9 kickstart[^2]: BaseOS / AppStream

Red Hat version specific repositories:

- Red Hat Enterprise Linux Server 7 x86_64: 7.0 / 7.1 / 7.2 / 7.3 / 7.4 / 7.5 / 7.6 / 7.7 / 7.8 / 7.9
- Red Hat Enterprise Linux for x86_64 8: 8.0 / 8.1 / 8.2 / 8.3 / 8.4 / 8.5 / 8.6 / 8.7 / 8.8 / 8.9 / 8.10
- Red Hat Enterprise Linux for x86_64 9: 9.0 / 9.1 / 9.2 / 9.3 / 9.4 / 9.5

Red Hat Product repositories:

- Red Hat Ansible Automation Platform
  - Red Hat Automation Hub 4.2 for RHEL 7 x86_64 (RPMs)
  - Red Hat Automation Hub 4.2 for RHEL 8 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.1 for RHEL 8 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.2 for RHEL 8 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.2 for RHEL 9 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.3 for RHEL 8 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.3 for RHEL 9 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.4 for RHEL 8 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.4 for RHEL 9 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.5 for RHEL 8 x86_64 (RPMs)
  - Red Hat Ansible Automation Platform 2.5 for RHEL 9 x86_64 (RPMs)

- Red Hat OpenShift Container Platform
  - Red Hat OpenShift Container Platform 4.10 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.11 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.12 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.12 for RHEL 9 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.13 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.13 for RHEL 9 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.14 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.14 for RHEL 9 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.15 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.15 for RHEL 9 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.16 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.16 for RHEL 9 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.17 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.17 for RHEL 9 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.18 for RHEL 8 x86_64 (RPMs)
  - Red Hat OpenShift Container Platform 4.18 for RHEL 9 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.12 for RHEL 8 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.13 for RHEL 8 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.14 for RHEL 8 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.14 for RHEL 9 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.15 for RHEL 9 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.16 for RHEL 9 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.17 for RHEL 9 x86_64 (RPMs)
  - Logical Volume Manager Storage 4.18 for RHEL 9 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.11 for RHEL 8 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.12 for RHEL 8 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.12 for RHEL 9 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.13 for RHEL 8 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.13 for RHEL 9 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.14 for RHEL 9 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.15 for RHEL 9 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.16 for RHEL 9 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.17 for RHEL 9 x86_64 (RPMs)
  - Ironic content for Red Hat OpenShift Container Platform 4.18 for RHEL 9 x86_64 (RPMs)

- Red Hat Satellite
  - Red Hat Satellite 6.10 (for RHEL 7 Server) (RPMs)
  - Red Hat Satellite 6.11 (for RHEL 7 Server) (RPMs)
  - Red Hat Satellite 6.11 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite 6.12 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite 6.13 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite 6.14 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite 6.15 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite 6.16 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite 6.16 for RHEL 9 x86_64 (RPMs)
  - Red Hat Satellite Capsule 6.10 (for RHEL 7 Server) (RPMs)
  - Red Hat Satellite Capsule 6.11 (for RHEL 7 Server) (RPMs)
  - Red Hat Satellite Capsule 6.11 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite Capsule 6.12 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite Capsule 6.13 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite Capsule 6.14 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite Capsule 6.15 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite Capsule 6.16 for RHEL 8 x86_64 (RPMs)
  - Red Hat Satellite Capsule 6.16 for RHEL 9 x86_64 (RPMs)

[^1]: Enabled by default when enabling Red Hat repositories.
[^2]: Enabled by default when enabling a Red Hat release repository.

## Requirements and Dependencies

Ansible Core 2.13.0 or higher is required for the roles in the collection.

The roles in this collection must be imported by the `kangaroot.foreman` collection. It is possible to directly use the roles in this collection but not recommended.

The `kangaroot.foreman` collection requires the `theforeman.foreman` and `theforeman.operations` collections. To install the required collections, execute:

```shell
ansible-galaxy collection install -r requirements.yml
```

in the collection directory.

## Collection Variables

The group_vars directory contains example vars files for the important variables used in the collection roles.

## Usage

The variable `foreman_content_roles` from the `foreman` role in the `kangaroot.foreman` collection contains a list content roles to import.

Add this collection content role to the `foreman_content_roles` list of content roles to import in your playbook project variables.

For example, add the `foreman_content_roles` variable in your `group_vars/foreman.yml` file of your playbook project:

```yaml
# Foreman content roles to include
foreman_content_roles:
  # Package only content
  - ...

  # OS content
  - kangaroot.foreman_content_redhat.foreman_content_redhat
  - ...

  # Builtin content
  - kangaroot.foreman_content_builtin.foreman_content_builtin
```

Also ensure that the Red Hat repositories are enabled by setting the appropriate enable variables:

```yaml
foreman_enable_redhat: true
```

In your playbook, add a task to execute the `kangaroot.foreman.foreman` role:

```yaml
- name: Run kangaroot.foreman roles
  hosts: foreman
  roles:
    - kangaroot.foreman.foreman
```

