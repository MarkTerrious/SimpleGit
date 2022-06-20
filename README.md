# SimpleGit
How to use git as a simple. == Git Tutorial

# Enviroment
   you can simply set this config after or before creating folder
the case before, it is used to all folder.

Local <br>
- git config user.name
- git config user.email
  
Global (including "") <br>
- git config --global user.name "MarkTerrious" <br>
- git config --global user.email "_____@gmail.com" <br>

# Remote
```
git remote add __RemoteNickNameAboutURL__ __RemoteURL__            // Connect with Specific Remote Repository
git remote -v                                                      // show all of remote repositroy url
git remote rename __From_RemoteNickName__ __To_RemoteNickName2__   // change nickname ex) origin -> main 
```   
# Create Project Folder
```
mkdir __   // project name at __  
cd __      // move to folder that you just created before
```
# Init
```
git init             // init
ls .git              // confirm it's made
ls ~/.gitconfig      // for Local, confirm how to config
ls -a                // search including hide file
```  
# Start the project
   ---------------------- Untracked -------------------------------
```
git clone __RemoteURL__ __NickName__   // bring data from gitHub
git add __FileName__                   // track specific file or folder name
git add .                              // track all of file and folder
git status                             // check modified status
```

```
git rm --cached __FileName__     // make files (here : __FileName__) on stage untracked (not commited)
git reset HEAD __FileName__      // make files untracked (already commited)
```
   ----------------------- tracked --------------------------------
```
git commit -m "__Commit_Message__"     // commit with message

/* in this case, you should commit once as a normal way before using this command option. */
git commit -am "__Commit_Message__"    // move file and foler to stage and try to commit. 
```
   
# Git Commited log
```
git log   // confirm git local repository
```   
# Pattern
```
git remote add __nickname__ __remoteURL__       // At Folder, connect gitHub (already lots of files or folders is) 
git clone __RemoteURL__ __NickName__            // To Folder, clone data from gitHub (empty folder)
```
