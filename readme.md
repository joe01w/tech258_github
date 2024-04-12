# Tech 258
## Github

#### What is version control? 
Version control is the ability to track changes made on a project, as people and teams collaborate on projects together.
<br>This is done through a VCS, or a version control system. A VCS tracks the history of changes.
<br> This means that when developers make changes to the project, any earlier version of the project can be recovered at any time.

Developers can review project history to find out:
* Which changes were made?
* Who made the changes?
* When were the changes made?
* Why were changes needed?

#### What is git, how does it work? 
Git is a version control system that tracks changes in files. It maintains a record of modifications, enabling collaboration and easy reversal of changes. 
It works by taking snapshots of the project's files and allows users to merge changes made by multiple contributors. 
The snapshot system means the git is more efficient and uses less resources than other VCSs.

### Showcase the basic git command flow. Explain what each command does and showcase the expected output: 

`git init` 
<br>This command to initialize a new repository. When you run git init in a directory, Git creates a new .git subdirectory inside that directory, which contains all the necessary files for the repository. 
This includes configuration files, object databases, and other metadata.
<br>

`git status` 
<br>This command displays the current state of the repository. 
When you run git status, Git provides information about which files have been modified, which files are staged for commit, and which files are untracked.

`git add` 
<br>This command used in Git to add changes in the working directory to the staging area. The staging area is a temporary storage area where you can prepare changes before committing them to the repository.
When you run git add, you specify the files or directories you want to add to the staging area.

`git commit` 
<br> This command is used to save the changes you've made to the files in your repository. 
When you run git commit, you create a new commit containing the changes that were previously staged using git add.
A commit in Git represents a snapshot of the repository at a particular point in time.

### Showcase what `git log` and `git diff` do 

`git log`
<br> This command displays the commit history of a repository. 
When you run git log, Git presents a chronological list of commits, starting with the most recent commit and proceeding backwards in time.

`git diff`
<br>This command is used to display the differences between the changes in the working directory and the changes that have been staged but not yet committed (in the staging area).

### What is `.gitignore` and why should we use it?
This command act as a blacklisting feature, so certain files or directories in a Git repository can be ignored.
This can be so Git doesn't recognize temporary folders, or folders with sensitive information.

## Task 1: Create a program that checks if a user can watch a movie based on the users age.

possible film ratings are "universal", "pg", "12", "12a", "15", "18"
<br> `film_rating = "12a"`

<br>Use an if statement to check for "universal" rating
<br> `if film_rating == "universal":
    print("all age groups can watch this film")`
<br>Checks if the film rating is "pg"
<br>`elif film_rating == "pg":
    print("General viewing, but some scenes may be unsuitable for young children.")`
<br>Checks if the film rating is "12" or "12a"
<br>`elif film_rating == "12" or film_rating == "12a":
    print("Films classified 12A and video works classified 12 contain material that is not generally suitable for children aged under 12. No one younger than 12 may see a 12A film in a cinema unless accompanied by an adult.")`
<br>Checks if the film rating is "15"
<br>`elif film_rating == "15":
    print("No one younger than 15 may see a 15 film in a cinema.")`
<br>Checks if the film rating is "18"
<br>`elif film_rating == "18":
    print("No one younger than 18 may see an 18 film in a cinema.")`
<br>Else statement if none of the above conditions are met
<br>`else:
    print("This is not a correct rating, please use universal, pg, 12, 12a, 15, 18")`



