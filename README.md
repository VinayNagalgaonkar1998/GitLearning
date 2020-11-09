# GitLearning
This is a repo consisting of a Java project to learn about Git 

### Git and GitHub

#### <u>Git</u>
Git is a free and open source distributed version control system designed to 
handle everything from small to very large projects with speed and efficiency.

#### <u>GitHub</u>
GitHub, Inc. is an American multinational corporation that provides hosting 
for software development and version control using Git.

### Git Commands

1. **git init**   
Description - To initialise a git repo for a new or existing project.

2. **git add <file_name>**  
Description - Add one or more files to staging (index). Using git add . will add all the modified 
and un-tracked files to the staging area.

3. **git status**  
Description - Lists the files you’ve changed and those you still need to add or commit.

4. **git commit -m “some commit message”** 
Description - Commit changes to HEAD.

5. **git commit -am “some commit message”**  
Description - Adding all un-staged files to staging area and commit changes to HEAD.
(Note : Works for modified files and not files that are un-tracked i.e. newly created files)

6. **git commit --amend**  
Description - The command is a convenient way to modify the most recent commit. It lets you combine 
staged changes with the previous commit instead of creating an entirely new commit. 
It can also be used to simply edit the previous commit message without changing its snapshot.

7. **git restore --staged <file_name>**   
Description - To un-stage said files from the staging area. However, restore command is generally used 
to discard changes without the --staged tag like ‘git restore <file_name>’. The following 
command is much more preferable to un-stage file.
    
8. **git rm --cached <file_name>**  
Description - To remove files from the Staging area.

9. **git log**  
Description - The command allows you to view information about previous commits that have occurred in a project. 
The simplest version of the ‘log’ command shows the commits that lead up to the state of the 
currently checked out branch

10. **git branch <branch_name>**  
Description - To create a new branch with name as ‘branch_name’

11. **git checkout <branch_name>**  
Description - To switch from current branch to another 

12. **git merge <branch_name>**  
Description - To merge a branch into current branch

13. **git remote add <alias_name> <GitHub_url>**  
e.g. git remote add origin https://github.com/VinayNagalgaonkar1998/GitLearning2.git
Description - Here, ‘origin’ is the name of the alias on our system for a particular remote repository hosted on 
say GitHub, GitLab or GitFarm (in the above case GitHub)

14. **git push <alias_name> <branch_name>**  
e.g. git push origin master   
Description - The git push command is used to upload local repository content to a remote repository. 
Pushing is how you transfer commits from your local repository to a remote repo. It's the 
counterpart to git fetch

15. **git push -u <alias_name> <branch_name>**  
e.g. git push -u origin master   
Description - The ‘git push -u’ command is equivalent to -set-upstream. The -u flag is used to set origin 
as the upstream remote in your git config. The above command will set the master branch as 
the default remote branch. (Using the example)The branch ‘master’ is set up to track remote 
branch ‘master’ from origin. So after running ‘git status’ we get message like 
“Your branch is up to date with 'origin/master'.” with respect to tracking

16. **git pull --rebase**  
Description - The ‘git pull’ command is used to fetch and download content from a remote repository and 
immediately update the local repository to match that content.   
However, it is a best practice to use the following version of git pull :  
git pull --rebase  
Reason - https://stackoverflow.com/questions/2472254/when-should-i-use-git-pull-rebase  
Another usage example of git pull --rebase :  
git pull --rebase origin br1FromMaster 

17. **git stash**  
Description - ‘git stash’ temporarily shelves (or stashes) changes you've made to your working copy so 
you can work on something else, and then come back and re-apply them later on. Stashing is handy 
if you need to quickly switch context and work on something else, but you're mid-way through a 
code change and aren't quite ready to commit.  
Use  
git stash pop  
to reapply previously stashed changes

18. **git reset HEAD~**  
Description - git reset command is a powerful command that is used to undo local changes to the state 
of a git repo. HEAD~ extension will take us back to one commit behind. It is equivalent to 
git reset HEAD\~1 and git reset HEAD\~n will take us ’n’ commits behind 

19. **git rebase --continue**  
Description - Rebase is one of two Git utilities that specialises in integrating changes from one 
branch onto another. The other change integration utility is git merge. The continue is most used up 
till now, thus the command is shown with this tag.

![Git rebase](https://drive.google.com/uc?id=1PlKgGESNMLEAiavBSoTS7GJhG4oaN0uz)