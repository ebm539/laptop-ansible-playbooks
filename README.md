# laptop-ansible-playbooks
Ansible playbooks for my laptop. Like dotfiles, but at the machine level, not at the user level.


TODO:
- identify installed software on laptop (e.g. browse systemd services and targets)
- convert current files in to jinja2 templates where necessary
- write Ansible playbooks that will output config for software


e.g. I'm planning to write playbooks that will put a network bridge into various states (IPv4 only, dualstack, IPv6-only, IPv6 single stack + NAT64/DNS64, and with & without ULA and default routes).
(This network bridge is to simulate various 'real world' networks that exist, to test software and hardware)

I'm also planning to write a playbook that is run on receiving a DHCPv6 prefix delegation, to create correct configuration files (from templates) for software that uses the delegated prefix (e.g. radvd) so I don't modify the files myself manually.
