# CLOUD ENGINEERING ASSIGNMENT

1. Create a User

Created a user called 'Diane'.

2. Set an expiry date of 2 weeks for the user

Set an expiry date of 2 weeks which is the 1st of September, 2023.
![Alt text](<Creating a user with expiry date of 2 weeks (1st Sept 2023).jpg>)

Set User password
![Alt text](<Set user password.jpg>)

3. Prompt the user to change the password on login

To verify: 'sudo chage -l Diane'.

From the output of the 'chage' command, it is seen that the user's password must be changed.
![Alt text](<Prompt the user to change the password on login.jpg>)

4. Attach the user to a group called 'altschool'

Created a group called 'altschool' and attached the user to the group.
![Alt text](<Attach the user to a group called altschool.jpg>)

To verify that the user 'Diane' is assigned to the 'altschool' group, ran 'groups Diane'

![Alt text](<To view the groups a user is assigned to.jpg>)

5. Allow 'altschool' group to be able to run only cat command on /etc/

Running 'sudo visudo' to open the 'sudoers' file

![Alt text](<Running sudo visudo.jpg>)

To the 'sudoers' file, added the line that will allow members of the 'altschool' group to use the 'cat' command on files within the '/etc/' directory.

![Alt text](<Allow altschool group to be able to run only cat command on etc.jpg>)

6. Create another user. Make sure that this user does not have a home directory

Created a user called 'testuser' without a home directory.

![Alt text](<Create user without home directory.jpg>)
