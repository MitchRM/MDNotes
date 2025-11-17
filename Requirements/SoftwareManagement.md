# Robot software management strategy
- **main** - The all correct version of robot software - will be saved at the end of the target robot's usefull life
- **develop** branch off **main** -
- **comp** branch off **main** - The branch to use during competition and events. A correct branch with some modifications made and tested during competion. 
- **feature** branch off **develop** : When work on the feature is ready for integrated testing Mitchell, Sr, or Matt will review the changes and merge in to develop.
- **working** branch off of feature : This is where you do your work. Keep all the work focused on the associated feature. When the work is complete merge it to the feature branch and delete the **working** branch. The work can be tested on the robot by building and deploying this branch.
## At the end of your work period or meeting, push your changes to the origin on Github to back up your work.
# Before you start working always make sure you are working on the right branch.