Playbook: inventory2csv
=======================

Sometimes it is easier to discuss about whats running on which machine or which machine belongs to which groups by using something like excel.

This Playbook can help you with this. It outputs all Hosts and the groups of the used inventory as csv file. There might be other scripts and tools and more sophisticated ways to do this ... this is my approach.

Tags:
-----
_N/A_

Variables:
----------
| Variable | Default | Purpose |
| -------- | ------- | ------- |
| file | ./output.csv | File where the generated CSV should be stored |

Example:
--------
```bash
ansible-playbook inventory2csv.yml -i inventory -e "file=./someotherfile.csv"
```

__Author__  
Mario Engels  
sysiphos@gmail.com