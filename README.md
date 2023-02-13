# StackOverflow Tags Prediction

The large stackoverflow dataset is pushed using GIT-LFS:

## How to use git-lfs?

Install [git-lfs](https://git-lfs.com/) for macos:

    brew install git-lfs

To ensure that git-lfs is setup correctly in your git configuration files use the git lfs install command:

    git lfs install


To make sure your large datafiles are tracked, this will track all the files with specified extension and uploads those files to Git's Large File Storage:

    git lfs track "*.zip"

Make sure to also add `.gitattributes` file while commiting your changes:

    git add .gitattributes

Voila! Git - LFS setup is done. You can go ahead and add, commit and push your changes.

You will get the following message while pushing,

    Uploading LFS objects: 100% (4/4), 1.8 GB | 726 KB/s, done.


## Accessing the zip files:

Now, normally do `git clone` to clone the repository

    git clone git@github.com:ii-varsha-ii/stackoverflow-tags-prediction.git

Now do `git lfs pull` to fetch and download the latest LFS files:

    git lfs pull

