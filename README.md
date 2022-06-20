# SimpleGit
How to use git as a simple. == Git Tutorial

1. Enviroment
   you can simply set this config after or before creating folder
the case before, it is used to all folder.

Local
  git config user.name
  git config user.email
  
Global (including "")
  git config --global user.name "MarkTerrious"
  git config --global user.email "_____@gmail.com"

Remote
   # Connect with Specific Remote Repository
   git remote add __RemoteNickNameAboutURL__ __RemoteURL__  
   # show all of remote repositroy url
   git remote -v      
   # change nickname ex) origin -> main
   git remote rename __From_RemoteNickName__ __To_RemoteNickName2__
   
2. Create Project Folder
  mkdir __      // project name at __
  cd __         // move to folder that you just created before
  
3. Init
  git init
  ls .git           // confirm it's made 
  ls ~/.gitconfig   // for Local, confirm how to config
  ls -a             // search including hide file
  
4. Start the project
   ---------------------- Untracked -------------------------------
   git clone __RemoteURL__ __NickName__ 
   git add __FileName__             // track specific file or folder name
   git add .                        // track all of file and folder
   git status                       // check modified status
   
   {
      // didn't commit yet
      git rm --cached __FileName__     // make files (here : __FileName__) on stage untracked

      // already commited
      git reset HEAD __FileName__      // make files untracked
   } 
   ----------------------- tracked --------------------------------
   git commit -m "__Commit_Message__"     // commit with message
   
   {
      # in this case, you should commit once as a normal way before using this command option.
      git commit -am "__Commit_Message__"    // move file and foler to stage and try to commit. 
   }
   
5. Git Commited log
   git log                          // confirm git local repository
   
# Pattern
# At Folder, connect gitHub (already lots of files or folders is) 
git remote add __nickname__ __remoteURL__
# To Folder, clone data from gitHub (empty folder)
git clone __RemoteURL__ __NickName__
