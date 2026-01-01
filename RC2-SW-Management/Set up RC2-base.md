# Set up RC2-base
## Set up RC2-base-local with scandisk server
Copied 6744-Reefscape-Development-development from GitHub - the current version on 28Dec2025
1. Cloned the development branch to a zip file and opened in tempory folder on my PC
2. Created bare repo on scandisk
   * Created new repo folder in scandisk GitServer folder
     * `PS D:\GitServer> mkdir -p RC2-base-local.git`
   * Made the folder a bare repo
     * `PS D:\GitServer\RC2-base-local.git> git init --bare`
3. Cloned the new bare server repo from scandisk to my PC
   * In RobotPrograms\Git-scandisk 
     * `git clone D:\GitServer\RC2-base-local.git` :
     * `git pull`     (Not sure this is needed since the server had nothing to pull)
4. Copied the Reefscape code into RC2-base-local repo using VSCode
   * Opened the temporary folder in VSCode
   * Opened the RobotPrograms\Git-scandisk\RC2-base-local.git in a separate VSCode window
   * Copied the files from the temporary folder to the new empty repo
5. Used Git to commit and push the changes from RC2-base-local on my PC to RC2-base-local origin on scandisk
   * `git add .`
   * `git commit -m "Initialize from 6744-Reefscape-Develoment-Development"`
   * Apparently there were many LF replaced by CRLF (?), because there were a bunch of warnings on the git add .
6. Did a build — it failed 
   * 
