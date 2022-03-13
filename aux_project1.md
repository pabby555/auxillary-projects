# AUX PROJECT 1
## Title: SHELL SCRIPTING
### TASK: 
This Project describes how 20 new Linux users were onboarded onto a server.

<!-- Horizontal Rule -->
------------------------------------

1. STEP ONE: Created a project folder named Shell
<!-- Code Blocks -->
```bash
$ mkdir Shell
$ cd Shell 
```
Creating Shell directory
![creating Shell directory](./images-aux-prj1/creating-shell-directory.png)

<!-- Horizontal Rule -->
------------------------------------

2. STEP TWO: Created a csv file names.csv to store user names in Shell directory
<!-- Code Blocks -->
```bash
$ touch names.csv
$ vim names.csv
```
Creating file names.csv
![creating names.csv file](./images-aux-prj1/creating-shell-directory.png)

<!-- Horizontal Rule -->
------------------------------------
3. STEP THREE: Created developers group
<!-- Code Blocks -->
```bash
$ groupadd developers
$ cat /etc/group | grep "developers"
```
Creating "developers" group and verifying it was successfully created
![creating developers group](./images-aux-prj1/creating-developer-group.png)

<!-- Horizontal Rule -->
------------------------------------

4. STEP FOUR: Updating current ubuntu user with public and Private keys
<!-- Code Blocks -->
```bash
$ cd .ssh
$ touch id_rsa.pub
$ touch id_rsa
$ vim id_rsa.pub
$ vim id_rsa
```
Creating id_rsa.pub and id_rsa files and adding the keys.
![Creating id_rsa files](./images-aux-prj1/creating-id_rsa-files.png)

![Editing id_rsa file](./images-aux-prj1/id_rsa.private-file.png)

![Editing id_rsa.pub file](./images-aux-prj1/id_rsa.pub-file.png)

<!-- Horizontal Rule -->
------------------------------------

5. STEP Five: Creating Script, adding execution permission for ubuntu user to run script, and finally running script.
<!-- Code Blocks -->
```bash
$ vim onboarding_users.sh
$ chmod u+x onboarding_users.sh
$./onboarding_users.sh
```
Execution permission given to ubuntu user.
![Creating script and adding execution permission](./images-aux-prj1/creating-script.png)

Shell Script
![Shell script](./images-aux-prj1/shell-script.png)

Script was successful. New users in /etc/passwd file.
![Running script ](./images-aux-prj1/verifying-successful-execution-script.png)

<!-- Horizontal Rule -->
------------------------------------

Testing onboarded users connections.

![testing connections ](./images-aux-prj1/testing-user-connections.1.png)

![testing connections ](./images-aux-prj1/testing-user-connections.2.png)

![testing connections ](./images-aux-prj1/testing-user-connections.3.png)