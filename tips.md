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

### To Add the permission to a user
setfacl -m u:user:rwx /path
setfacl -m u:raman:rwx /tmp/test
### To Add the permission to a group
setfacl -m g:group:rw /path
setfacl -m g:ec2-user /tmp/dir
### To allow all the files or directories to inherit ACL entries from the directory it is within
TBS
### To remove the permission for a specific user
 setfacl -x u:raman test
### To remove all the entries 
 setfacl -b test
<b>Note </b> -w option not allow to delete the directory/file but you can modify

# Help Commandsh
1. <b>whatis</b>  it gives very minimal information like <i>whatis touch </i>
2. <b>help</b> it gives gives descriptive information of a command <i>ls --help </i>
3. <b>man</b> it gives more descriptive command 


