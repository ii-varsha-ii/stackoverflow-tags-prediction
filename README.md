# StackOverflow Tags Prediction 

## Final Report : https://docs.google.com/document/d/13yaVhUEDIfmfNJTsGj0eleVrHcbwm9d8q6hIE2JpjqQ/edit?usp=sharing

## Problem Statement
The StackOverflow platform is used by millions of users to post questions, provide answers or even search answers for questions posted by the user. While posting the questions users can assign tags that are closely related to the question.
The problem space we have taken up is to use StackOverflow Dataset to predict tags of the questions posted. A efficient way for tagging is necessary since adding tags to questions manually is a burden to the user and reduces the overall user experience of the website. Hence, we are planning to use machine learning to assign tags to questions

## Approach
Multilabel classification is used to predict the relevant tags for the questions. 
` Multi-label Classification allows the model to classify items in datasets with more than one target variable. A given instance may belong to more than one label when making predictions, hence making it non-mutually exclusive. `
Since a question in StackOverflow can be associated with multiple tags, this problem comes under a multi-label classification domain.

## Dataset:
Stackoverflow dataset: https://www.kaggle.com/datasets/stackoverflow/stacksample 

## Developer guide:
The large stackoverflow dataset is pushed using GIT-LFS:

### How to use git-lfs?

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


### Accessing the zip files:

Now, normally do `git clone` to clone the repository

    git clone git@github.com:ii-varsha-ii/stackoverflow-tags-prediction.git

Now do `git lfs pull` to fetch and download the latest LFS files:

    git lfs pull

