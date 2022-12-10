# laptop-ansible-playbooks
Ansible playbooks for my laptop. Like dotfiles, but at the machine level, not at the user level.


TODO:
- identify installed software on laptop (e.g. browse systemd services and targets)
- convert current files in to jinja2 templates where necessary
- write Ansible playbooks that will output config for software


e.g. I'm planning to write playbooks that will put a network bridge into various states (IPv4 only, dualstack, IPv6-only, IPv6 single stack + NAT64/DNS64, and with & without ULA and default routes).
(This network bridge is to simulate various 'real world' networks that exist, to test software and hardware)
