# ansible-ssh
Connect to Ansible hosts using the Ansible inventory.

**Usage**

    ansible-ssh PATTERN [COMMAND]
    
Where PATTERN can be the name of a single host as specified in you inventory files, 
a group name, or regular expression. In other words, I just pass the given pattern 
to Inventory.get\_hosts() and let Ansible figure it out. 
When PATTERN matches multiple hosts, it lets you connect to all of them sequentially.
When COMMAND is present, it gets executed just as it would have been using `ssh HOST COMMAND`.

# ansible-groups
Show all groups, or all groups matching PATTERN.

**Usage**

    ansible-groups [PATTERN]
    
Where PATTERN is a string that must be present in a groups name (case insensitive).

# ansible-hosts
An alternative for Ansibles's --list-hosts.
Show all hosts, or all hosts matching PATTERN.

**Usage**

    ansible-hosts [PATTERN]
    
Where PATTERN is a string that must be present in a groups name (case insensitive).
