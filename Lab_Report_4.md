# **Lab Report 4**
---
## Step 4 - Log into ieng6

![Code Image](lab-report-4-signinsc.png)

```
ssh cs15lfa23du@ieng6.ucsd.edu <enter>
```
Sign into ssh


## Step 5 - Cloning into ssh

![Code Image](lab-report-4-clone.png)
```
rm -r -f lab7 <enter>
```
Delete the previously saved repository

```
git clone git@github.com:arjunbhalla03/lab7.git
```
Clone the repository

## Step 6 - Run the Tests

![Code Image](lab-report-4-runtests.png)

```
cd lab7 <enter>
```
make the working directory lab7

```
bash test.sh <enter>
```
Run the JUnit tests scripts inside test.sh
