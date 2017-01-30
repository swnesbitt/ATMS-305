# Week 2 Issues Summary

Here are a few common issues from students:

## 1. When I try to use git, it says that this is not a repository, even though I did `git clone`

Your *working directory* needs to be within the repository. For example: `/data/atms305/a/netID/ATMS-305`.

If you are one directory up, `git` will not find the repository.  

Note that if you run `git clone`, you are not in the repository.  You need to `cd repositoryname` there.

**Tip:** use `pwd` to find your current working directory.

## 2. I can't find my `ATMS-305` directory, even though I cloned it when I logged in.

When you log into keeling, your home directory (`/data/keeling/a/netID`) is not your class directory (`/data/atms305/a/netID`).  Be sure to do your work for this class in the `/data/atms305/a/netID` directory.  Use the `cd` command to get there.  Use the `ls` command to list what is in a directory.

## 3. How and where should I save my answers for HW1?

**This is my bad.**  Please save your terminal output using copy/paste in a text file called `responses.txt` in a directory `Week2Answers` in the directory `/data/atms305/a/netID/ATMS-305`. One way to do this:
```bash
cd /data/atms305/a/netID/ATMS-305
mkdir Week2Answers
cd Week2Answers
pico responses.txt
```
In windows, you can paste in `putty.exe` by highlighting something with the mouse (this automatically copies it), and then clicking the right mouse button to paste.
On a mac, you can use command-C, command-V.

## 4. I'm confused on when to use `cd` with the whole path or with just the name of a directory.

If you are one directory above a folder, you can simply type `cd foldername`.  For example, if there exists a directory `ATMS-305` in the directory `/data/atms305/a/netID` (verified with `pwd` and `ls` as necessary), then I can just type `cd ATMS-305` to enter that directory.  

If I am somewhere else on the file system, then I can to enter the full path name to go there, i.e.: `cd /data/atms305/a/netID/ATMS-305`.

Or I could do it in two steps:
```sh
cd /data/atms305/a/netID/
cd ATMS-305
pwd
> /data/atms305/a/netID/ATMS-305
```
