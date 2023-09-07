### good first issue
#### Alphabets and Numbers have gone missing

Fix the issue, By following the given instructions.

### Development workflow

Branches are one of the basic concepts of git. There is a main branch `main` (previously `master`), and new branches are created out of the main branch. Every branch represents a feature you are working on, and it has different series of commits. Once a feature is complete, the feature branch is `merged` into the main branch.

Branches allow us to work on more than 1 feature at the same time, thus helping us avoid mixing of commits. If during the process, there are useless commits added and the whole branch is messed up, you can easily delete the branch and create a fresh branch from the `main` branch.

Note: **Never ever commit or rebase on your main branch**.

The development workflow goes like this :

1. Clone the repo.
2. Cd into the repo.
3. Currently, you are on your `main` branch. Now you need to change the 'Alphabet.txt' and 'numbers.txt' , Create a new branch with:    

    `git branch <branch-name>`    
    And then, checkout to the branch you created by:
    
    `git checkout <branch-name>`
    This brings you to your new branch \<branch-name>.
    
4. Now, edit the 'Alphabet.txt' and 'numbers.txt' and fix the missing letters and correct the order. When you have made the changes, `commit`.

    The process of commiting goes like this:
    
    `git status` : This shows the status of your files, i.e. it shows which files are present in the staging area and which are not.
    
    `git add <path/to/file>` : This adds the selected files to the staging area. To add, all the files to staging area, do `git add .`
    
    `git commit` : On doing this, a text editor opens up and you are asked to enter a commmit message. Commit message should be short (less than 50 characters), and should convey what change you have made. Keep the commit message as meaningful as possible.
    
5. You have successfully committed your changes. You can then push these changes to your remote repository by :
    `git push origin <branch-name>`.    
    Note that all these changes took place in your created branch \<branch-name> , and you can delete whatever changes you made by deleting the branch. The above command pushed youur code online to your github repository.
    
6. Go to github's online repository and you can see an option of `Compare and Pull request` against your recently pushed branches. Make a Pull request by entering a short meaningful message and a meaningful comment about what your pull request does.
