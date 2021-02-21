# Git 
## Explainning Git 

In order to explain Git, we have to first explain what Version Control is:

Version Control is a system that allows you to revisit various versions of a file or set of files by recording changes. Through version control, one can revert a file or project to a previous version, track modifications and modifying individuals, and compare changes. By utilizing a Version Control System (VCS), mistakes with files can easily be rectified.

## So, what is Git?

### Snapshots

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.


### Tracking Changes

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.



### operations 

`git clone <repo URL>` , this used to clone a repo 
`git status` , to get the status on snapshots 
`git add`, add modified data to the staging area 
`git commit`, commit changes
`git push`, push changes on repo 
