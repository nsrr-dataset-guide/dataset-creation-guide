# Create a GitHub Repository

In order to allow multiple users to contribute and to easily sync with sleepdata.org, project documentation are hosted in individual GitHub repositories. These repositories are then cloned onto the sleepdata.org servers and shown to site visitors. Repositories should be named in a way that clearly indicate that it is the documentation for a particular project (e.g. [shhs-documentation](https://github.com/nsrr/shhs-documentation)). Repositories can be created in the following manner, through the GitHub web client:

 - Locate the `+` icon next to your user account
 - From the dropdown menu, select a `New Repository`
    - Note: If you are logged in under your personal account, you should change the owner to an organization, such as sleepepi
 - Name your repository, following the above-mentioned conventions, and select the option to "Initialize this repository with a README"
 - Do not choose to add a .gitignore or a license
 - After you create the repository, you will be taken to the repository's home page. On this page you will be able to find a 'clone url' on the right hand side. Note this url, as you will need to make a local copy of the repository later (example:`git@github.com:nsrr/shhs-documentation.git`)


If you have already uploaded your data dictionary into your repository, you will want to clone it (make a local copy) onto your computer using either command prompt or terminal. Instructions for doing this can be found [on the web](http://git-scm.com/book/en/Git-Basics-Getting-a-Git-Repository) and below:

```
informinion:code michael$ git clone git@github.com:nsrr/example-documentation.git
Cloning into 'example-documentation'...
remote: Counting objects: 3, done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Receiving objects: 100% (3/3), done.
Checking connectivity... done.
```
The above line of code, `git clone git@github.com:nsrr/example-documentation.git`, has created a folder called "example-documentation" on your computer to serve as a local copy of your data dictionary. It is in this local copy that you will be able to add new and modify existing pieces of documentation, before pushing updates out to the web.

### _Next: [Structure Your Documentation](structure_your_documentation.md)_
