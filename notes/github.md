## Add cloned repo to my github 
(https://stackoverflow.com/questions/18200248/cloning-a-repo-from-someone-elses-github-and-pushing-it-to-a-repo-on-my-github)
1. Create a new repository at github.com. (this is your repository)
  - Give it the same name as the other repository.
  - Don't initialize it with a README, .gitignore, or license.
2. Clone the other repository to your local machine. (if you haven't done so already)
  - ```git clone https://github.com/other-account/other-repository.git```
3. Rename the local repository's current 'origin' to 'upstream'.
  - ```git remote rename origin upstream```
4. Give the local repository an 'origin' that points to your repository.
  - ```git remote add origin https://github.com/your-account/your-repository.git```
5. Push the local repository to your repository on github.
  - ```git push origin master```
----------
##### Now 'origin' points to your repository & 'upstream' points to the other repository.

Create a new branch for your changes with ```git checkout -b my-feature-branch```.
You can ```git commit``` as usual to your repository.
Use ```git pull upstream master``` to pull changes from the other repository to your master branch.

## Add gitignore
https://stackoverflow.com/questions/19663093/apply-gitignore-on-an-existing-repository-already-tracking-large-number-of-files

# Issue labels
https://blog.adam-marsden.co.uk/better-github-labels-f1360b43e0a7
