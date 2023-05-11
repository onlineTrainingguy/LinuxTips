# Find and Locate
Both are used to find the location of the file . <b>find</b> commmand returns the relative path whereas <b>locate</b> returns the absolute path
## Note
If locate command is not found or it is not found then run following commands

1. rpm -qa | grep mlocate
2. yum install mlocate
3. locate test.sh
4. updatedb
5. locate test.sh

# Soft link and Hard link
1. ln for create hard link ( Hardlink works with in same partition)
2. Hard links are only for files
3. Deleting the source file will not impact the hardlink.
4. Soft links can be for files and directories
5. ln -s  create soft link (ln -s source  dest)
6. ls -i returns the node number

# File permission
1. x permission allow a directory to go inside if a directory does not have the x permission then we cannot go inside it.
2.  chmod a+x  where a indicates everyone.
3.  6- rw  5 wx 3 xw 2 w 1 x
4.  getfacl test will return
