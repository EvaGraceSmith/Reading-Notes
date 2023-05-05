[gitpractice](https://learngitbranching.js.org/)


### Lessons:

#### Level 1
___
* ##### git commit  ![Level 1-1](img/git-level-01-01.png)
    * git commit -m 'what you did for this commit'

* ##### git branches  ![Level 1-2](img/git-level-01-02.png)
    * git branch newBranch - creates a new branch
    * git checkout -b newBranchName - makes a new branch and moves you to it
    * git switch branchName(or git checkout branchName) -moves you to a different branch

* ##### git merge ![Level 1-3](img/git-level-01-03.png)
    * git merge branchName will merge the branchName with the branch you are currently on.

 * ##### git rebasing ![Level 1-4](img/git-level-01-04.png)
    * git rebase branchToMoveTo  - This command will move the commits of the branch you are currently on, to the branch you name. To fully combine you need to then move (checkout) to the branchToMoveTo and git rebase branchYouAreCurrentlyOn. 

#### Level 2
___
* ##### Moving around in Git  ![Level 2-1](img/git-level-02-01.png)
* HEAD is the commit you are working on top of
* *git checkout commitName* will move HEAD from a branch to a commit

* ##### Relative Refs  ![Level 2-2](img/git-level-02-02.png)
* Moving upwards one commit at a time with ^
* Moving upwards a number of times with ~<num>
* *git checkout main^* will move HEAD one generation up. ^^ will move it two, etc

* ##### Relative Refs #2  ![Level 2-3](img/git-level-02-03.png)
* *git checkout HEAD~4* will move HEAD up four spaces
* *git branch -f main HEAD~3*  moves (by force) the main branch to three parents behind HEAD.

* ##### Reversing changes in Git  ![Level 2-4](img/git-level-02-04.png)
* *git reset* reverses changes by moving a branch reference backwards in time to an older commit. LOCAL ONLY
* *git reset HEAD~1* moves reference back by 1 from Head
* *git revert branchName* works for remote branches


#### Level 3 - Moving Work Around
___
* #####  git cherry-pick ![Level 3-1](img/git-level-03-01.png)
* *git cherry-pick commitName commitName* adds commits from other branches onto your current branch


* #####  Interactive rebase ![Level 3-2](img/git-level-03-02.png)
* Discusses an interactive way to rebase using a command such as: *git rebase -i HEAD~4*
* This would be a good way to go through and remove and change the order of commits if you have one that has changes you do not want. 



#### Level 4
___
* #####  Locally Stacked Commits ![Level 4-1](img/git-level-04-01.png)
* Grabbing just one commit
* discusses using both rebase and cherry pick to select which commit to keep and move

* #####  Juggling Commits ![Level 4-2](img/git-level-04-02.png)
* How to alter a commit way up the chain:
* *git commit -i HEAD~2* re-order the commits so the one we want to change is on top with git rebase -i
* *git commit --amend* to make the slight modification
* *git rebase -i HEAD~2* re-order the commits back to how they were previously with git rebase -i
* *git rebase caption main* move main to this updated part of the tree to finish the level

* #####  Juggling Commits #2 ![Level 4-3](img/git-level-04-03.png)
* How to accomplish the same as above using cherry pick and no rebase:
* *git checkout branchYouWantToBeOn*
* *git cherry-pick commitYouWantToAmend* pick the commit you want to amend.
* *git commit --amend* Amend the commit.
* *git cherry-pick commitYouWantAtTheEndOfTheBranch*

* #####  Git Tags![Level 4-4](img/git-level-04-04.png)
* Tags exist as anchors in the commit tree that designate certain spots.
* 

* #####  ![Level 4-5](img/git-level-04-05.png)

#### Level 5
___
* #####   ![Level 5-1](img/git-level-05-01.png)

* 
* #####  ![Level 5-2](img/git-level-05-02.png)