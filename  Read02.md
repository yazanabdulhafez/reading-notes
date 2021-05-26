# Read: 02 - Revisions and the Cloud

## Git: 
**Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it.**

### Cloning:
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

**$ git clone URL**

By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it.

### local Repository Structure:
1. The local Git repository has three components:
Working Directory: The actual files reside here.
2. Index: The area used for staging
3. Head: Points to the most recent commit

### The Life Cycle of File Status:
1. After you edit a file, Git flags it as modified because of changes made after the previous commit.
2. You stage the modified file.
3. Then, you commit staged changes.

### Tracking and Staging a New File 

Single File:
Track one file only by using the following format:
git add filename

All Files

Track all files in a repository by using the following
command:

***$ git add . ***

After using these commands, files are tracked and staged for committing.

### Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message:

**$ git commit -m “made change x,y,z”.**
By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles. By using git remote -v, you can view all the remote URLs next to their corresponding short names.

### pushing a File
After commiting afile we can push it to GitHub with
this command

**$git push origin main**


### Remote Repositories
In order to collaborate on Git projects, you must interact with remote repositories, versions of a project residing online or on a network. You can work with multiple repositories, for which you can have read/write or read-only privileges. Teams can use remote repositories to push information to and pull data from.

 ### Cloned Repositories

As mentioned earlier, for cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local branch.

Seeing Your Remotes
By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.

By using git remote -v, you can view all the remote URLs next to their corresponding short names.**