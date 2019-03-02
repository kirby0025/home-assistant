# home-assistant

Just my own home-assistant config.
Heavy work in progress as I'm just started.

# Proxmox VM-LXC handling

Requirements

  * SSH access to proxmox host using key-authentication.
  * Proper sudoers right for hass user.
```bash
hass ALL=(ALL) NOPASSWD: /usr/sbin/qm status *
hass ALL=(ALL) NOPASSWD: /usr/sbin/qm shutdown *
hass ALL=(ALL) NOPASSWD: /usr/sbin/qm start *
hass ALL=(ALL) NOPASSWD: /usr/bin/lxc-info -s *
hass ALL=(ALL) NOPASSWD: /usr/bin/lxc-stop -W *
hass ALL=(ALL) NOPASSWD: /usr/bin/lxc-start *
```
