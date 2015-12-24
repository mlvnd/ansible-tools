# ansible-ssh
Connect to Ansible hosts using the Ansible inventory.

**Usage**

    ansible-ssh PATTERN [COMMAND]
    
Where PATTERN can be the name of a single host as specified in you inventory files, a group name, or regular expression. In other words, I just pass the given pattern to Inventory.get_hosts() and let Ansible figure it out. When PATTERN matches multiple hosts, it lets you connect to all of them sequentially.
When COMMAND is present, it gets executed just as it would have been using `ssh HOST COMMAND`.
