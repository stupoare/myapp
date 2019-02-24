# LEARN GIT CLI
##### Better late than never


## What I have done (and learned) :
1. `$ cd /Data/web/tests` - Go to a location on your computer
2. `$ mkdir myapp` - Create a folder
3. `$ cd myapp` - Go inside this new folder

4. Create some files inside app folder :  
   `$ touch index.html`  
   `$ touch app.js`  
   `$ touch style.css`  

5. `$ git init` - Create .git config directory
6. `$ git --global user.name 'Sorin Paun'` - config name
7. `$ git --global user.email 'stupoare@gmail.com'` - config email

8. **Must-know commands 1** (**add**, **status**, **rm**) :  
   `$ git add index.html` - "Stage" a file (ready to be commited/uploaded)  
   `$ git status` - See the status of your files  
   `$ git rm --cached index.html` - To "unstage" a file  
   `$ git add *.html` - Stage all .html files  
   `$ git rm --cached *.html` - Unstage all .html files  
   `$ git add .` - Stage ALL files  
9. If you change the content of a file while in "stage" area you have to add it again!

10. `$ touch .gitignore` - Added a ".gitignore": this is where you put folders and files you want to ignore!

11. **Must-know commands 2**  (**commit**, **branch**, **checkout**, **merge**) :  
   `$ git commit -m 'The commit commentary goes here'` - Commit with a comment  
   `$ git branch myapp-branch` - Will create a new branch with the name **myapp-branch**  
   `$ git checkout myapp-branch` - Will switch to *myapp-branch* branch  
   *Note: while in this branch, all changes will be within this branch !*
   
   `$ git checkout master` - Will switch back to master branch  
   `$ git merge myapp-branch` - Will merge this branch from master.

   If there are files in conflict (like README was changed while in myapp-branch) we'll see a message:  
   *Auto-merging README.md*  
   *CONFLICT (content): Merge conflict in README.md*    
   *Automatic merge failed; fix conflicts and then commit the result.*  
   Do a `$ git add .` and a `$ git commit -m 'bla-bla'` to fix conflicts and run git commit...  

12. **Must-know commands 3** :  
    `$ git remote add origin https://github.com/username/reponame.git` - Add all *myapp* local files to the remote repo with the name **reponame**.  
    `$ git push -u origin master` - Will push the files and folders to master repo *reponame*  
    *Note: If is the first time you do this, Github will ask you for the github username and password*  
    
13. After the first *push -u origin*, and so the origin is already defined, you only have to do:  
    * `$ git add .`
    * `$ git commit -m "Bla Bla"`
    * `$ git push`  

   in order to update the remote repository

## TO DO
   * Add git commands related to "**Pull Requests**" (from a brach)
   * Add users
   * "**Fork**" a project
   * ...

## Credits
   This great guy: Brad Traversy / [Traversy Media](https://www.youtube.com/user/TechGuyWeb/)  