# Set up RC2-base
## First set up RC2-base-local with scandisk server
### Copied 6744-Reefscape-Development-development from GitHub - the current version on 28Dec2025
- Cloned the development branch to a zip file and opened in tempory folder on my PC
### Created bare repo on scandisk
-  Opened scandisk GitServer folder in terminal
    - `PS D:\GitServer> mkdir -p RC2-base-local.git` 
        - To create new repo folder
- cd to new folder
    - `PS D:\GitServer\RC2-base-local.git> git init --bare`
        - To make the folder a bare repo
### Cloned the new bare repo from scandisk to my PC
- In RobotPrograms\Git-scandisk in terminal
    - `git clone D:\GitServer\RC2-base-local.git` : 
        - to clone server repo
    - `git pull`
        - Not sure this is needed since the server had nothing to pull
### Copied the Reefscape code into RC2-base-local repo using VSCode
- Opened the temporary file in VSCode
- Opened the RobotPrograms\Git-scandisk\RC2-base-local.git in a separate VSCode window 
- Copied the files from the temporary folder to the new empty repo
### Use Git to commit and push the changes from RC2-base-local on my PC to RC2-base-local origin on scandisk
- `git add .`
- `git commit -m "Initialize from 6744-Reefscape-Develoment-Development"`
    - Apparently there were many LF replaced by CRLF (?), because there were a bunch of warnings on the git add .