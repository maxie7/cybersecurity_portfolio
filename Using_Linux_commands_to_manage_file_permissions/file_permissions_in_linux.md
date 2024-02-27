## File permissions in Linux

### Project description

Our organization's research team necessitates adjustments to access privileges for specific files and directories under the projects folder. The existing permissions do not align with the appropriate authorization levels, posing potential security risks. Addressing this concern, I methodically undertook the following measures to fortify our system's security posture:

### Check file and directory details

The following code shows the Linux command to determine the existing permissions for a specific directory in the file system.

![check_details](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/a15d96d2-cf54-46b7-8f91-248889ae1fd0)

The screenshot shows the command I used to list the contents of the projects directory, and the output of the command.

I used the ls command with the `-la` option to list all contents of the projects directory, including hidden files. The output of the command shows that there is one directory named drafts, one hidden file named `.project_x.txt`, and five other project files. The permissions for each file or directory are shown in the first column.

The 10-character string in the first column represents the permissions set on each file or directory. The first character indicates the file type, followed by three characters for the permissions for the owner, three characters for the permissions for the group, and three characters for the permissions for others.

### Describe the permissions string

The 10-character string can be interpreted to determine who has access to the file and what permissions they have. The characters and their meanings are as follows:

- The first character indicates the file type. A d means the file is a directory, and a hyphen (-) means the file is a regular file.
- The next three characters indicate the read, write, and execute permissions for the file's owner. A r means the owner has read permissions, a w means the owner has write permissions, and an x means the owner has execute permissions. A hyphen (-) means the owner does not have any permissions.
- The next three characters indicate the read, write, and execute permissions for the file's group. The meanings are the same as for the owner's permissions.
- The last three characters indicate the read, write, and execute permissions for everyone else on the system. The meanings are the same as for the owner's and group's permissions.

For example, the file permissions for `project_t.txt` are `-rw-rw-r--`. The first character is a hyphen (-), so `project_t.txt` is a regular file. The second, fifth, and eighth characters are all r, so the owner, group, and everyone else all have read permissions. The third and sixth characters are both w, so only the owner and group have write permissions. No one has execute permissions for `project_t.txt`.

### Change file permissions

In accordance with the directives I received, I was tasked with revoking write privileges for the "other" group across all files within our system. Upon examining the access permissions for the "project_k.txt" file, I identified that the "other" group was granted unwarranted write access. To rectify this non-compliance and ensure adherence to the prescribed guidelines, I employed a series of Linux commands to surgically remove the write access privilege for the "other" group. The following code snippet exemplifies the precise steps I undertook to accomplish this critical security task:

![change_permissions](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/c0942d7b-7195-40ab-b89d-40b4bea09ee0)

The first two lines of the screenshot show the commands that I ran, and the other lines show the output of the second command. The chmod command is used to change the permissions on files and directories. The first argument to the chmod command specifies the permissions that should be changed, and the second argument specifies the file or directory that the permissions should be changed for. In this example, I ran the command `chmod o-w project_k.txt` to remove write permissions from other for the file `project_k.txt`. I then ran the command `ls -la` to review the changes that I had made.

### Change file permissions on a hidden file

The research team at my organization recently archived the file `project_x.txt`. They do not want anyone to have write access to this file, but the user and group should have read access. I used the following Linux commands to change the permissions for this file:

![change_permissions_hidden_file](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/d5d9d612-86da-4858-bf96-de7083778c60)

The first two lines of the screenshot show the commands that I ran, and the other lines show the output of the second command. I know the file `.project_x.txt` is a hidden file because it starts with a period (.). In this example, I removed write permissions from the user and group, and added read permissions to the group. 

### Change directory permissions

My organization only wants the user `researcher2` to have access to the directory drafts and its contents. This means that no one other than researcher2 should have execute permissions for the directory or its contents. I used the following Linux commands to change the permissions:

![change_dir_permissions](https://github.com/maxie7/cybersecurity_portfolio/assets/15796607/fd9f1f79-5f15-48b0-8874-46f0b717bb44)

The first two lines of the screenshot show the commands that I ran, and the other lines show the output of the second command. I had previously determined that the group had execute permissions for the directory drafts. To ensure that only the researcher2 user has execute permissions, I ran the command `chmod o-x drafts` to remove the x (execute) permission from the other user. The `researcher2` user already had execute permissions, so they did not need to be added.

### Summary

To align the access privileges across multiple files and directories within the projects folder with the authorization levels mandated by our organization, I embarked on a systematic process. The initial step entailed executing the "ls -la" command, which provided a comprehensive overview of the current permissions for the directory in question. This critical information guided my subsequent actions. Thereupon, I employed the "chmod" command repeatedly, meticulously adjusting the permissions for various files and directories, ensuring strict adherence to the guidelines stipulated by our organization. This comprehensive approach enabled me to methodically establish the desired security posture across the designated resources.
