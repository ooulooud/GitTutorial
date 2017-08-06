# GitTutorial

## Set up Git
### For Mac Terminal:
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

### For Xcode:
      1. Check out an existing project
      2. Enter a repository location
      3. In Finder, open with Xcode
      4. Source Control->Commit

Git [Cheat Sheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet/)

### Terminal commands:
      1. git clone https://github.com/ooulooud/GitTutorial.git
      2. cd GitTutorial
      3. git branch ssh_test     // create a new branch
      4. git checkout ssh_test   // switch to new branch
      5. git status
      6. git add README.md
      7. git commit -m "Added terminal commands"
      8. git push --set-upstream origin ssh_test

From github.com:

      1. Compare and Merge branch
      2. Delete local branch: git branch -d ssh_test

Sync foreign branch:

      1. git fetch
      2. git checkout ssh_update

### For C++ project:
      1. Create a repo on github WITHOUT any file including README.md. The repo must be empty.
      2. Create a new Xcode project, and check Create Git repository on My Mac.
      3. Source Control->Config->add remotes
      4. Source Control->Commit
      5. To import a github project: checkout an existing project
