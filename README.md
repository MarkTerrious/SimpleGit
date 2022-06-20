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
  1. Connect with Specific Remote Repository
  2. show all of remote repositroy url
  3. change nickname ex) origin -> main 
  
- git remote add __RemoteNickNameAboutURL__ __RemoteURL__            
- git remote -v                                                      
- git remote rename __From_RemoteNickName__ __To_RemoteNickName2__   
   
# Create Project Folder

1. project name at __
2. move to folder that you just created before

- mkdir __      
- cd __        
  
# Init
1. init
2. confirm it's made
3. for Local, confirm how to config
4. search including hide file

- git init
- ls .git           
- ls ~/.gitconfig    
- ls -a              
  
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
- git commit -m "__Commit_Message__"     // commit with message
   
   { <br>
      # in this case, you should commit once as a normal way before using this command option.
      git commit -am "__Commit_Message__"    // move file and foler to stage and try to commit. 
   } <br>
   
# Git Commited log
   git log                          // confirm git local repository
   
# Pattern
- At Folder, connect gitHub (already lots of files or folders is) 
git remote add __nickname__ __remoteURL__
- To Folder, clone data from gitHub (empty folder)
git clone __RemoteURL__ __NickName__
