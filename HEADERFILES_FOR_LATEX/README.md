# The central header files repository

This repository comprises all newly defined commands, all newly defined environments, all used packages and explanations for each of those within the respective tech files.
It also has an up-to-date version of our logo.
Working like that we can be sure that all of us produce compatible latex code which adheres to the same style maximes.

# How ?

1. Go to the folder that contains your current documentation project.
    The folder including your chosen template is one of the folders presented on the [templates project](https://gitlab.ethz.ch/ARIS/Documentation/Templates).
    
 The folder structure should look like this:
    
    - Documentation_Project
        - Folder_Of_Your_Chosen_Template

2. Invoke `git submodule add https://gitlab.ethz.ch/ARIS/Documentation/HEADERFILES_FOR_LATEX.git`

    This command will add a folder called HEADERFILES_FOR_LATEX to your structure. From this point on you will be able to compile your project.
    
 The folder structure should now look like this:
    
    - Documentation_Project
        - Folder_Of_Your_Chosen_Template
        - HEADERFILES_FOR_LATEX

# Advanced stuff

It is even possible to make a change to your local version of the header files and push that change to this repo.

__Notice that your documentation must always comply with the central header files, it will not be accepted when handed in if it doesn't!__

1. Make your change
2. `cd HEADERFILES_FOR_LATEX`
3. `git checkout -b feature_branch` where feature_branch shall be some meaningful name for your intended addition to the header files.
4. `git add .` to add all proposed changes.
5. `git commit -m "your nice message"` with a really nice message, clearly describing what you changed and why! Follow [this](https://chris.beams.io/posts/git-commit/)!
6. `git push --set-upstream origin feature_branch` where again you replace feature_branch with your meaningful name.
7. Come back here again end create a [pull request](https://gitlab.ethz.ch/ARIS/Documentation/HEADERFILES_FOR_LATEX/branches) for your branch.