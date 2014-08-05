# Create a GitHub Repository

In order to allow multiple users to contribute to data dictionaries, the data dictionaries are hosted in individual GitHub repositories. These repositories are then cloned onto the sleepdata servers and overlayed on the datasets. Repositories should be named in a way that clearly indicate that it is the data dictionary for a particular projects (e.g. [shhs-data-dictionary](https://github.com/sleepepi/shhs-data-dictionary)). Repositories can be created in the following manner, through the GitHub web client:

 - Locate the `+` icon next to your user account
 - From the dropdown menu, select a `New Repository`
    - Note: If you are logged in under your personal account, you should change the owner to an organization, such as sleepepi
 - Name your repository, following the above-mentioned conventions, and select the option to "Initialize this repository with a README"
 - Do not choose to add a .gitignore or a license
 - After you create the repository, you will be taken to the repository's home page. On this page you will be able to find a 'clone url' on the right hand side. Note this url, as you will need to make a local copy of the repository later (example:`git@github.com:sleepepi/shhs-data-dictionary.git`)


After creating the repository, you will want to clone it (make a local copy) onto your computer using either command prompt or terminal. Instructions for doing this can be found [on the web](http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository) and below:

```
informinion:code michael$ git clone git@github.com:sleepepi/example-data-dictionary.git
Cloning into 'example-data-dictionary'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Receiving objects: 100% (3/3), done.
Checking connectivity... done.
```
The above line of code, `git clone git@github.com:sleepepi/example-data-dictionary.git`, has created a folder called "example-data-dictionary" on your computer to serve as a local copy of your data dictionary. It is in this local copy that you will be able to create new variables and make changes to existing ones, before pushing updates out to the web
