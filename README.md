Task 2: Number Guessing Game



main:



Initial branch of game with base features. User can guess the random generated number with generic feedback.



feature1:



Based on main branch. Adds quit feature and tells user how to use quit feature. Also allows user to play again.



feature2:



Based on dev branch. Additional features include: user has max attempts to guess the number and the max attempts is a constant number.



feature3:



Based on main branch. Additional feature of improved hints to user when guessing.



hotfix:



Based on main branch. The maximum number in the range can now possibly be the random number.



dev:



Based on main branch. Additional feature: an encouraging message to players when they start the game.



documentation:



Based on feature1 branch. Documentation creation through work progress.



Learning Summary:



Merge: combines branches and keeping all branch history.



Rebase: applies commits from one branch to another by creating a cleaner, more linear history.



Squash: combines many commits into 1 to reduce clutter.



Cherry-Pick: apply very specific commits from one branch to another instead of the whole thing.



Branch Observations:



The feature1 branch commits are part of the dev branch as feature1 was deleted. This is a result of merging.



The feature2 branch was rebased on from main to dev. By doing this, the git log history of feature2 contains commits made in dev, feature2, and feature3.



The feature3 branch based on the main branch. It was rebased, squashed, and merged onto dev. By doing so, the vague commit messages were \*almost\* completely fixed. There was an issue when I did it resulting in a duplication. By doing this, feature3 has less commits than before and is more comprehensible.



The hotfix branch was based on main and was cherry-picked onto dev. In the tree, it is not shown that hotfix is connected back to dev because only one line was cherry-picked. It was merely taking a commit from hotfix and applying it to the other branch. If it had been merged, it would be connected.



The documentation branch is still not connected back to anything. I imagine it does not need to be for this assignment. So in this case, this branch is shown like a loose leaf similar to the hotfix branch.



I would use merge when I have completed a number commits and want to keep all commit history.



I would use rebase when I have completed a number of commits on a branch, but I want to condense the commits when sharing with another branch for a more linear history.



I would use cherry-pick when I do a minor bug fix that does not require a substantial change to the entirety of the program. This way, I do not have to merge everything and resolve a number of merge conflicts.



I would use squash when I have a number of commits that are related and could be combined into one commit so that a task is not so dissected. This way, my git log history can be cleaner.

