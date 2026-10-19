# Ancora-Education-Ucertify-Lab52
# Managing Group Accounts

> **Original Lab Source**
> 
> This lab was available through:
>
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=5]

## Objective of the Lab 
In this lab, you will learn to manage group accounts. Groups in Linux are important because users are present on the system for a defined utility. Grouping users by utility (or access) is a fantastic way to ensure that only admins have admin privileges and that general users can only access files that they are meant to. 
## Instructions 
### STEP 1 
From the left sidebar, open the Terminal window. 
### STEP 2 
Execute the following command to display the current user’s ID and group membership:
```bash
id
```
### STEP 3
Execute the command to display the group membership of the root account:
```bash
groups root
```
### STEP 4
Execute the following command to determine the user owner and group owner of the /etc/group file:
```bash
ls -l /etc/group
```
### STEP 5
Execute the following command to display the group account information for the games group:
```bash
grep games /etc/group
```
### STEP 6
Execute the following command to display the group password information for the games group:
```bash
grep games /etc/gshadow
```
### STEP 7
Execute the following command to switch to the root account:
```bash
su -
```
### STEP 8
Execute the following command to create a new group named test:
```bash
groupadd test
```
### STEP 9
Execute the following command to display the group account information for the test group:
```bash
grep test /etc/group
```
### STEP 10
Execute the following command to change the group name of the test group to newtest:
```bash
groupmod -n newtest test
```
## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.
