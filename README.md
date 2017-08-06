# GitTutorial
Git tutorial

Set up Git
For Mac Terminal:
1. Download Git from https://git-scm.com/download/mac
2. Allow the installation of thrid-party package. 
   System Preferences->Security & Privacy->unlock->open anyway->open the package->lock. 
3. Open terminal and type git --version
4. Config identification
   git config --global user.name "ooulooud"
   git config --global user.email "ooulooud@gmail.com"
   // Setup HTTPS
   git config --global credential.helper osxkeychain
5. Setup SSH
   Check for existing public keys: ls -al ~/.ssh
   Generate new key: ssh-keygen -t rsa -b 4096 -C "ooulooud@gmail.com"
   Copy public key to clipboard: pbcopy < ~/.ssh/id_rsa.pub and add to Settings->SSH and GPG keys->New SSH key

For Xcode:
1. Check out an existing project
2. Enter a repository location
3. In Finder, open with Xcode
4. Source Control->Commit

Git Cheat Sheet:
https://services.github.com/on-demand/downloads/github-git-cheat-sheet/

Terminal commands:
1. git clone https://github.com/ooulooud/GitTutorial.git
2. cd GitTutorial
3. git branch ssh_test     // create a new branch
4. git checkout ssh_test   // switch to new branch
5. git status
6. git add README.md
7. git commit -m "Added terminal commands"
8. git push --set-upstream origin ssh_test
