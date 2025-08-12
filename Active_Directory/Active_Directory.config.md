# AD
- Created and Managed OU's for Admins and Users
- Applied GPO'S to enforce password and login restrictions
- Automated the creation of 1000 test user accounts via powershell

Admins OU created:


<img width="751" height="524" alt="Active Directory Users and Computers Pic" src="https://github.com/user-attachments/assets/31f0f4ca-51c6-40b6-8231-9fd2f84eb023" />


Created the Admins OU and set username style to first letter of first name + last name

The powershell script used for the 1000 test user accounts:

<img width="1023" height="723" alt="CREATE USER SCRIPT PICTURE" src="https://github.com/user-attachments/assets/b742cd6d-a600-4a57-a114-1c362103f7aa" />

"_USERS" OU created in Active Directory, Script sets the same password for all users, Loop made for all users being evaliated, the loop will split the user's name between first and last, then in the first initial + full last name format, a username will be created. "password never expires" box will be checked on, then the information is to directed in the _USERS folder in the AD, the account then gets enabled.


The 1000 test user accounts list:

<img width="752" height="526" alt="Active Directory 1000 User's Pic" src="https://github.com/user-attachments/assets/30cd08b8-394a-4a68-8cef-c4945fcc5397" />


To ensure that the Windows client was successfully registered on the Active Directory:


<img width="752" height="528" alt="Active Directory Computers List" src="https://github.com/user-attachments/assets/2bab1708-f5ff-47f0-baea-0da8eae4e126" />
