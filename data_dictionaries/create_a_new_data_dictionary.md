# Create a New Data Dictionary

Creating a data dictionary from scratch using Spout is simple. In your command line (either command prompt for Windows or Terminal for Mac), just navigate to the location where you would like to place the local copy of your data dictionary, and use the command `spout new $data-dictionary-name`, where $data-dictionary-name is the name of your project's data dictionary. An example of this code is shown below:

```
informinion:examples michael$ spout new example_data_dictionary
      create  .gitignore
      create  .ruby-version
      create  .travis.yml
      create  .spout.yml
      create  Gemfile
      create  Rakefile
      create  domains
      create  domains/.keep
      create  variables
      create  variables/.keep
      create  forms
      create  forms/.keep
      create  test
      create  test/dictionary_test.rb
      create  test/test_helper.rb
         run  bundle install
```
This code and output shows the Spout creating a new data dictionary template, including the necessary GitHub files, in the location of your choice. After you create your data dictionary, you will want to link it to the GitHub repository you created for it online. To do so, use the following code below:

```
informinion:example-data-dictionary michael$ git init
Initialized empty Git repository in /Users/michael/code/examples/example-data-dictionary/.git/
informinion:example-data-dictionary michael$ git remote add origin git@github.com:mcailler/example-data-dictionary.git
```
- Please note that you should replace`mcailler/example-data-dictionary.git` with the SSH url of your own repository, which can be found on GitHub.
- When you link your repository using this method, you will need to use the special command `git push -u origin master` when making your first commit. Afterwards, you will be able to use the standard `git push`

Many of Spout's features will be discussed in later sections of this guide, but if you run into any issues installing or using Spout, you can find support at the GitHub repository for it: [https://github.com/sleepepi/spout](https://github.com/sleepepi/spout)
