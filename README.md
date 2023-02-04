# Practice-PR-Playlists
Practice creating pull requests with a list of playlists.
(With thanks to [https://github.com/bhargav794/hacktoberfest-practice-music-playlists](https://github.com/bhargav794/hacktoberfest-practice-music-playlists))

## To start ...
Create an account on Github, and make sure you have the following installed:

* [Git](https://git-scm.com/downloads)
* A dev environment to handle .md files
    * [VS Code](https://code.visualstudio.com)
    * [Notepad++](https://notepad-plus-plus.org)

## What's next?
### In brief:
Have a look at [Github's Fork & Pull Workflow for Git Beginners](https://reflectoring.io/github-fork-and-pull/) for an overview of this process. However, here is a simple list of things to do:
(In particular, checkout 'Updating your Fork'  for information on mking sure you push the latest version of the repo)

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this project
2. Open Git Bash
3. [Clone]() your forked project 
    ```sh 
    git clone https://github.com/<YOUR-USERNAME>/Practice-PR-Playlists
    ```
4. Make your changes to the `playlist.md` file
5. Add the URL of your spotify playlist
6. [Add](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository) the file to the staging area:
    ```sh
    git add .
    ```
7. [Commit](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository) your changes. Include a commit message to describe your commit:
    ```sh
    git commit -m "YOUR COMMIT MESSAGE"
    ```
8. [Push](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository) the changes to your forked version.
    ```sh
    git push origin main
    ```
9. Go to the original project (i.e . my project!) on GitHub and create a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

### More detailed descriptions of the steps
1. Fork this repo.
2. `clone` your forked copy of the project
     ```sh 
    git clone https://github.com/<YOUR-USERNAME>/Practice-PR-Playlists
    ```
3. In git bash, change the working directory to inside the cloned project:
    ```sh
    cd Practice-PR-Playlists
    ```
4. Add a reference to the original (i.e. my) repository:
    ```sh
    git remote add upstream https://github.com/markdoughty/Practice-PR-Playlists.git
    ```
5. Check the remote repositories
    ```sh
    git remote -v
    ```
6. Use `git pull` to make sure the upstrwam remote repository (i.e. mine) is up to date with your fork:
    ```sh
    git pull upstream main
    ```
7. Create a new branch in your repository:
    ```sh
    git checkout -b <YOUR-BRANCH-NAME>
    ```
8. Open `Playlist.md` in a code editor like VSCode or notepad++ and make your changes. To add a Spotify playlist reference, use this markdown syntax:
    ```sh
    [playlist name](Spotify URL of the playlist)
    ```
9. Add your files to your staging area (track your changes):
    ```sh
    git add .
    ```
10. Commit the files in the staging area:
    ```sh
    git commit -m "YOUR COMMIT MESSAGE"
    ```
11. `push` the committed files to your repository (i.e. your forked version):
    ```sh
    git push -u origin <YOUR-BRANCH-NAME>
    ```
12. Create a `pull request`. Select 'Pull Requests > Create Pull request'. Please ensure you compare your branch to the branch of the repository (i.e. mine) to which you want to make a pull request.
13. Wait to see whether it is merged into the main branch!

    



