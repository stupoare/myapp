# LEARN GIT CLI
> Better late than never


## What I have done (and learned) :
1. __`$ cd /Data/web/tests`__ - Go to a location on your computer
2. __`$ mkdir myapp`__ - Create a folder
3. __`$ cd myapp`__ - Go inside this new folder

4. Create some files inside app folder :  
   __`$ touch index.html`__  
   __`$ touch app.js`__  
   `$ touch style.css`  

5. __`$ git init`__ - Create .git config directory
6. __`$ git --global user.name 'Your Name'`__ - Config name
7. __`$ git --global user.email 'username@domain.com'`__ - Config email

8. __Must-know commands 1__ (`add`, `status`, `rm`) :  
   __`$ git add index.html`__ - "Stage" a file (ready to be commited/uploaded)  
   __`$ git status`__ - See the status of your files  
   __`$ git rm --cached index.html`__ - To "unstage" a file  
   __`$ git add *.html`__ - Stage all .html files  
   __`$ git rm --cached *.html`__ - Unstage all .html files  
   __`$ git add .`__ - Stage ALL files  
9. If you change the content of a file while in "stage" area you have to add it again!

10. __`$ touch .gitignore`__ - Added a ".gitignore": this is where you put folders and files you want to ignore!

11. **Must-know commands 2**  (`commit`, `branch`, `checkout`, `merge`) :  
   __`$ git commit -m 'The commit commentary goes here'`__ - Commit with a comment  
   __`$ git branch myapp-branch`__ - Will create a new branch with the name *myapp-branch*  
   __`$ git checkout myapp-branch`__ - Will switch to *myapp-branch* branch  
   *Note: while in this branch, all changes will be within this branch !*  
   `$ git checkout master` - Will switch back to master branch  
   `$ git merge myapp-branch` - Will merge this branch from master.

      If there are files in conflict (a file was changed while in myapp-branch) we'll see a message:  
      *Auto-merging \<filename\>*  
      *CONFLICT (content): Merge conflict in \<filename\>*    
      *Automatic merge failed; fix conflicts and then commit the result.*  
      Do a `$ git add .` and a `$ git commit -m 'bla-bla'` to fix conflicts and run git commit...  

12. __Must-know commands 3__ (`remote` `origin`, `push`):  
    __`$ git remote add origin https://github.com/username/reponame.git`__ - Add all *myapp* local files to the remote repo with the name *reponame*.  
    __`$ git push -u origin master`__ - Will push the files and folders to master repo *reponame*

    *Note: If is the first time you do this, Github will ask you for the github username and password*  
    
13. After the first *push -u origin*, and so the origin is already defined, you only have to do:  
    * __`$ git add .`__
    * __`$ git commit -m "Bla Bla"`__
    * __`$ git push`__  

   in order to update the remote repository

## TO DO
   - [ ] Add git commands related to "**Pull Requests**" (from a brach)
   - [ ] Add users
   - [ ] `fork` a project
   - [ ] :metal:

## Credits
   This great guy: Brad Traversy / [Traversy Media](https://www.youtube.com/user/TechGuyWeb/)  