# ansible-cheat-sheet
ansible-cheat-sheet

#####how to run a particular task on specific host in ansible
If you want to run your role on all hosts but only a single task limited to the webservers group, then - like you already suggested - when is your friend.

You could define a condition like:

when: inventory_hostname in groups['webservers']
