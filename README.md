# Connecting _Github_ and _Git_ using _VsCode_

## What is Github?
GitHub is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code


## Terms used in Github and git

1. Git
   > Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

2. Version Control System
   > describes a type of software that is designed specifically to help manage the complexities - and so much more!

   ### Advantages of Version Control
   + Automatically create a backup of your work
   + Provide an easy way to undo mistakes and restore a previous version of your work
   + Document changes with a log that describes what's been changed and why
   + Keep file names and hierarchies consistent and organized
   + Branch work off into multiple "sandboxes" (called branches in Git) that allow developers to experiment without impacting other branches
   + Collaborate with others without disturbing each other's or our own work
  
3. Repository(or _repo_ in short)
   >  A directory of files that are tracked by Git.

4. Track
   > When a file is tracked by Git, it means that Git will notice any changes to that file. We call these changes differences or **diffs**. Git allows you to choose whether to **commit** a diff in order to keep it.

5. Diff
   > The diff of a file is all the changes that have been made to it since the last commit. The diff of a repo is all the diffs in all the tracked files in the repo that have not yet been committed (sometimes programmers call this the **_diffset_**)

6. Commit
   >Once we decide we want to save a **diff**, we commit the diff to the repo's history using the commit command. When we make a commit, we write a _log message_ that describes what happened in the diff. The set of commits provides a history of all of the changes that have been made to a repo and when.

7. Log
   >A record of what happened in each commit.

8. Local/Remote
   > Local refers to the _repo_ on our personal system the local repo.Remote refers to the repo hosted on **GitHub**

9. Branch/default branch
    > A Git repo can support multiple branches that make it possible for multiple developers to be working on the code at the same time.When you initialize a new Git repo a default branch is created (**_main_**) where your work will be tracked by default.

10. Pull Requests
    > These are hearts of collaborations. With a pull request you are proposing that your changes should be merged with the main branch from your branch..

### Creating a New Branch
```
git branch <Branch name>

```
### switching to another branch that does not exitst specifying it shoud be created using -b
```
git checkout -b <branch name>
```
### switching to an already existing branch
```
git checkout <branch name>
```

    
## Softwares You Need and how to download them
1. ### Softwares
   > + Git
   > + VsCode

2. ### Installations
    1. ### Windows
         -  ### **VsCode**
            > Navigate to this Website [_here_](https://code.visualstudio.com/download)
         -  ### **Git**
            >Navigate to this Website [_here_](https://git-scm.com/)
         

    2. ### Linux
        - ### **VsCode**
            ```
            sudo apt update
            sudo apt upgrade
            sudo apt install code
            ```
            >if this does not work install vscode manually using this link [_here_](https://code.visualstudio.com/download)
            > if you still insist on installing using the terminal then read this article and follow the instructions [_here_](https://phoenixnap.com/kb/install-vscode-ubuntu)
        - ### **GIT**
            ```
            # apt-get install git
            # add-apt-repository ppa:git-core/ppa 
            # apt update
            # apt install git
            ```

## Useful VsCode extensions
+ How to install vscode extensions:
    1. From Extensions > Manage Extensions, find the extension you want to install. (If you know the name or part of the name of the extension, you can search in the Search window.)
    2.  Select Download.
+ Must have extensions:
    1. colorize
    2. Prettier
    3. icon fonts
    4. live server
    5. bracket pair colorizer
    6. js ES6 snippet
    7. live share extension

## Creating a Github Account
+ if you have not sign-up proceed to this url [Github signup webpage](https://github.com/join)
+ Fill out the form and create an account
+ verify Email Address connected to your Github Account
  
if you were able to verify email address, continue below
## Configure Git and GitHub
[Git](https://git-scm.com/download/linux) is the tool we use to download and upload our code online. To use Git without signing every time, you need to create a Secure Shell (SSH) key and associate that to your GitHub account.
#### **_Follow the steps below and everything will be done:_**
 > ### Steps 
 1. Open the terminal in your vsCode or gitbash in windows or press <code>ctrl + `</code> on linux
 2. Type <code>git config --global user.name</code> + <code>Space</code> + your name and press <code>Enter</code>. (**Note** _this should be your full name, not your GitHub username, in quotes_)
 3. <code>Type git config --global user.email</code> + <code>Space</code> + the email address you used to sign up to GitHub and press <code>Enter</code>
 4. Type <code>git config --global init.defaultBranch main</code> to update the default branch name to **_main_**
 5. Type <code>ssh-keygen and press</code> <code>Enter</code>.For each prompt do not type anything, just continue to press <code>Enter</code>. It's particularly important that you do not enter a passphase; you should leave the passphrase empty when prompted.
 6. Type <code>cat ~/.ssh/id_rsa.pub | clip.exe</code> and press <code>Enter</code>. This will copy your SSH key to your clipboard
 7. Open the [Github New SSH key form ](https://github.com/settings/ssh/new) (**_NOTE_**: You need to be logged in to access this link)
 8. Type _"My personal PC"_ in the "Title" input field
 9. Paste what's on your clipboard from step six in the "Key" input field
 10. Click "**Add SSH Key**"

If you see your new SSH key beneath the "SSH keys" heading You have finally managed to configure your github...

### Enjoy

