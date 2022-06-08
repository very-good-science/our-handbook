Before a Workshop
====

Things to do before attending a workshop.

````{admonition} Group Leaders
We expect that the different members of your group may have different levels of experience with git and GitHub.
It would be helpful for us if each group could identify a "Group Leader" who is most experienced with GitHub - this is your leader just for the handbook - they will have some extra setup tasks and will be responsible for setting up your team's Handbook repository. 

````

If you don't have any experience with git or GitHub don't worry - we will be able to help on the day.

Remember to bring your laptop and a charger!

Group Members
----
For group members (i.e. everyone in your group):
 - create a GitHub account if you don't already have one
 - familiarise yourself with Markdown:
      - [GitHub Markdown guide](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
 - (optional) you may also like to familiarise yourself with git:
      - [Introduction to git](https://chryswoods.com/introducing_git/)
      - [Collaborating with git](https://chryswoods.com/git_collaboration/)


Group Leaders
----
The group leader will need basic familiarity with git.

````{admonition} For Group Leaders Only
Only one person per group (the Group Leader) needs to follow the instructions below.

````

For the group leader:
 - create a GitHub account for your organisation
 - [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this [repository](https://github.com/very-good-science/our-handbook)
 - make sure your team has access to your fork


### Setting up python
You will need to have python installed on your computer to build the webpages.
You can install the required python modules by running the following in a terminal:

```
pip install -U -r requirements.txt

```

from the root directory of your repo.


### Building your Handbook
You may also like to build your handbook locally so that you can see your changes.
 - clone your repository
 - check that you are working on the main branch and bring in any new changes
     - `git checkout main`
     - `git pull`
 - (optional) create a feature branch
     - `git checkout -b group-away-day-page`
 - make any edits that you want to view
 - build the site to make sure any changes are as you expect
     - go to the root of your respository and run `jb build book/`
     - after completion, you can open `book/_build/html/index.html` to view the webpage
 - save, commit and push

