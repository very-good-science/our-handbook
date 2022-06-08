# Contributing to the `Our Handbook` template

Welcome to `Our Handbook`, a template for a Research Group handbook and materials to help you make use of it. 
These materials are under continuous development, and will continue to
take shape around your suggestions, so we really welcome you to share your ideas.

Please follow our [Code of Conduct](code-of-conduct) in all spaces where Our Handbook members are interacting.


## Browser vs. Local machine

There are two ways to suggest changes to the project via [GitHub](https://github.com/): using your internet browser, or using your local machine.
In these contribution guidelines, you will sometimes see instructions labelled __in the browser__ or __on your local machine__ referencing these two different ways of doing things.
If you need help with either of these methods, please [open a new Discussion](https://github.com/very-good-science/our-handbook/discussions/new) and we'll be happy to help!

If you're comfortable using the terminal and Git (or you're interested in learning), then we recommend __using your local machine__.
This means you:

- Will have a copy of the project files on your computer
- Can make changes using your favourite text editor
- Can preview what your suggested handbook pages will look like
- __But__ it requires a little more set up

If today's not the day that you want to dig into Git and the terminal, then you can still contribute __via the GitHub website__ in your usual internet browser.
This means you:

- Don't need to install anything on your computer
- Don't need to use a terminal
- __But__ you won't be able to preview how things will look on the `Our Handbook` website.

```{seealso}
If you'd like to know more about using Git and the terminal, then we recommend [The Turing Way's chapter on Version Control](https://the-turing-way.netlify.app/reproducible-research/vcs.html) to get started.
```

## Step-by-step

Here's a step-by-step guide for contributing to this project through GitHub. 
If you have any problems with any part of this process or you'd like further explanation, please [open a new Discussion](https://github.com/very-good-science/our-handbook/discussions/new) and we'll be happy to help!

1. Getting ready
2. Let us know what you're working on
3. Copy (_fork_) the project
4. Make some changes
5. Create a _pull request_
6. Tell us you're finished

### 1. Getting Ready

Firstly, you need a GitHub account to contribute.

- [Sign up for a GitHub account](https://github.com/signup) if you don't have one yet.

Secondly, decide what you'd like to work on!

- Check out our [Open Issues](https://github.com/very-good-science/our-handbook/issues) for inspiration.
- We have a few [Good First Issues](https://github.com/very-good-science/our-handbook/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) labelled, which might be a good place to start.
- If you're not sure what you'd like to do, then we're happy to help.  We can chat about that on [this discussion](https://github.com/very-good-science/our-handbook/discussions/24).
   
### 2. Let us know what you're working on

By telling us what you're working on, we can avoid duplicating effort, and make sure we can direct everyone's energy into the best output for the project.

- If you find an existing issue that you want to work on, comment on it and tell us that you're working on it.

### 3. Copy (_fork_) the project

You will work on your own copy of the project, called a _fork_.
This means if you accidentally make a mistake, or you have work in progress, you don't need to worry about overwriting anything, because it won't affect the central version until you're ready to show us.

When you create a fork, you make your own copy of the project's files (called a _repository_ or _repo_) in your GitHub account.

````{tab} In the browser
If this is the first contribution you've made to the repository, then follow [these instructions](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository) to fork the repository for the first time.

- [This](https://github.com/very-good-science/our-handbook) is the repository that you want to fork

```{note}
If you've made a fork of the repository before, for an earlier contribution, then now you need to _sync_ it, since your existing forked copy is probably a little out of date. 

- [Follow these instructions](https://docs.github.com/en/github/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) to sync your fork
```
````

````{tab} Using your local machine
To get a copy of all the project files on your local machine you must first fork the repository (see instructions for 'In the browser') and then `git clone` **your fork** of the repository.
Cloning just means copying the project files to your local machine.
After cloning, open a terminal in the root of the our-handbook directory and install the necessary dependencies.

- Clone **your fork** of the repository using either of the following commands:
    - `git clone https://github.com/YOUR_USER_NAME/our-handbook.git`
    - `git clone git@github.com:YOUR_USER_NAME/our-handbook.git`
- Change to the directory for your newly cloned repository: `cd our-handbook`
- Create and activate a [virtual environment](https://docs.python.org/3/library/venv.html) using your preferred tool
- Run `pip install -r requirements.txt`

```{note}
If you already cloned the repository earlier, then you will instead need to pull the latest changes to the `main` branch.
You may also need to install any updated dependencies using inside your virtual environment.
- [Sync your fork](https://docs.github.com/en/github/collaborating-with-pull-requests/working-with-forks/syncing-a-fork) of the repository on GitHub
- Use `git checkout main` and `git pull` to get the latest changes from your synced fork
- And `pip install -U -r requirements.txt` to update the dependencies
```

```{seealso}
[Here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) are some general instructions for cloning a repository, and [here](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository) shows an example of cloning a fork.
```
````

### 4. Make some changes
Now you're ready to make some changes and save or _commit_ them to your forked repository.
 

```{tip}
Check our [style guide](style-guide) for advice on how to add content to the template, including how to add instructions to handbook authors (the users of the template).
```

````{tab} In the browser

1. Go to __your fork__ on GitHub `github.com/YOUR_USER_NAME/our-handbook`
2. Find the file that you want to edit
    - Most files you will want to edit will be in `book/guide` or `book/template`
    - If it doesn't exist, you can [create a new file](https://docs.github.com/en/repositories/working-with-files/managing-files/creating-new-files) make sure it has the file suffix `.md`
3. Edit the file
    - Click the pen symbol to open the file editor
    - Make changes formatted in the MyST Markdown language
    - You can preview changes, which will show you the general size of headings, but they won't be able to show some of the fancier MyST commands
4. Save or _commit_ regularly
    - When you've made a change (even if small), scroll down to where it says "Commit changes", and type a short meaningful message describing the change you made - we recommend committing changes regularly (every 20 minutes or so)
    - Click "Commit changes"
````

````{tab} Using your local machine
1. Check that you are working in the `main` branch and sync any changes made by others
    - `git checkout main`
    - `git pull`
2. (Optional) you may wish to create a _feature branch_ off the `main` branch
    - For example, `git checkout -b add-group-away-days-page`
3. Open the file that you want to edit in your favourite text editor
    - Website content is in either `book/guide` or `book/template`
    - Create a new `.md` file if needed
4. Edit the file
    - Make changes in MyST Markdown
5. Build the site to check that it looks as you expected
    - To check how the site looks, go to the root of the repository and run: `jb build book/`
    - After completion, you can open `book/_build/html/index.html` to view the website
    - Please check your changes display correctly before marking your _pull request_ as ready for review (see below)
6. Save, commit, and push to your fork regularly
    - `git commit`
    - `git push`
````

```{seealso}
`Our Handbook` is a [jupyter book](https://jupyterbook.org/) which means that all the content for the book is written in MyST Markdown: you can find a useful cheat sheet [here](https://jupyterbook.org/reference/cheatsheet.html).
```

### 5. Create a _pull request_

A _pull request_ tells us where to look for changes you are making.
You can wait until all your changes are made before creating your pull request, but it is really helpful if you create one as soon as you start making changes.
Creating a __draft__ pull request up front shows us what is actively being worked on, and it also helps you get feedback early into making your changes.
When you add more commits, your draft pull request will automatically update.

- Create a pull request from your forked repository to the `main` branch of the `Our Handbook` repository
- We recommend you create a __draft__ pull request as early as possible
- Please fill out our Pull Request template as best you can

```{seealso}
You can follow [these instructions](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) to create the Pull Request. 
```

### 6. Tell us you're finished
It's the final step!
All that's left to do is [mark your pull request as ready to review](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/changing-the-stage-of-a-pull-request#marking-a-pull-request-as-ready-for-review).

A member of the `Our Handbook` team will check your changes to make sure that we can bring them into our main repository.
At this time we're likely to start talking by leaving comments on your pull request, and hopefully your changes will soon be ready to merge in!
