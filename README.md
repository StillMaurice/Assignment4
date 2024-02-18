# Assignment4
Assignment update





- Your login name: altschool i.e., home directory /home/altschool. The home directory contains the following sub-directories: code, tests, personal, misc Unless otherwise specified, you are running commands from the home directory.

- Change directory to the tests directory using absolute pathname

- Change directory to the tests directory using relative pathname

- Use echo command to create a file named fileA with text content ‘Hello A’ in the misc directory

- Create an empty file named fileB in the misc directory. Populate the file with a dummy content afterwards

- Copy contents of fileA into fileC

- Move contents of fileB into fileD

- Create a tar archive called misc.tar for the contents of misc directory

- Compress the tar archive to create a misc.tar.gz file

- Create a user and force the user to change his/her password upon login

- Lock a users password

- Create a user with no login shell

- Disable password based authentication for ssh

- Disable root login for ssh


 - ## Solutions

a. `cd /home/altschool/tests`

b. `cd tests`

c. `echo 'Hello A' > /home/altschool/misc/fileA`

d. `touch /home/altschool/misc/fileB && echo 'Dummy content' > /home/altschool/misc/fileB`

e. `cp /home/altschool/misc/fileA /home/altschool/misc/fileC`

f. `mv /home/altschool/misc/fileB /home/altschool/misc/fileD`

g. `tar -cf /home/altschool/misc/misc.tar /home/altschool/misc`

h. `gzip /home/altschool/misc/misc.tar`

I. `useradd -m -s /bin/bash newuser && passwd -e newuser`

J. `passwd -l username`

K. `useradd -M -s /sbin/nologin userwithnologin`

L. `sed -i 's/#PasswordAuthentication yes/PasswordAuthentication no/' /etc/ssh/sshd_config`
