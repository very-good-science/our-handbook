# Contributing to the `Our Handbook` project

Welcome to `Our Handbook`, thank you for your interest in growing this project!

The `Our Handbook` project is a template for a Research Group handbook and materials to help you make use of those. 
The project is currently very early in development, and will take shape around your suggestions, so we really welcome you to share your ideas.

Please follow our [Code of Conduct](code-of-conduct) in all spaces where Our Handbook members are interacting.

````{admonition} E-life Innovation Sprint
If you're joining us for the E-life Innovation Sprint 2021, hello and welcome!
I've put together some specific information for you about our aims, availability and where to can chat to us [over here](./elife-sprint).
````

## Browser vs. Local machine
There are two ways to suggest changes to the project via GitHub: using your internet browser, or using your local machine.
In these contributing guidelines, you will sometimes see instructions labelled __in the browser__ or __on your local machine__ referencing these two different ways of doing things.
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
We're also happy to walk you through getting set up if you'd like some extra support.
```

## Step-by-step

Here's a step-by-step guide for contributing to this project through GitHub. 
If you have any problems with any part of this process or you'd like further explanation, please [open a new Discussion](https://github.com/very-good-science/our-handbook/discussions/new) and we'll be happy to help!

1. Getting ready
2. Let us know what you're working on
3. Copy the project
4. Create a draft "Pull Request"
5. Make your changes
6. Tell us you're finished

### 1. Getting Ready

Firstly, if you don't have one yet, then [sign up for a GitHub account](https://github.com/signup).

Secondly, decide what you'd like to work on!
- Check out our [Open Issues](https://github.com/very-good-science/our-handbook/issues) for inspiration. 
- We have a few [Good First Issues](https://github.com/very-good-science/our-handbook/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) labelled, which might be a good place to start.
- If you're not sure what you'd like to do, then we're happy to help.  We can chat about that on [this discussion](https://github.com/very-good-science/our-handbook/discussions/24).
   
### 2. Let us know what you're working on
By telling us what you're working on, we can avoid duplicating effort, and make sure we can direct everyone's energy into the best output for the project.
If you find an existing issue that you want to work on, comment on it and tell us that you're working on it.

### 3. Copy the project
You will work on your own copy of the project.
This means if you accidentally make a mistake, or you have work in progress, you don't need to worry about overwriting anything, because it won't affect the central version until you're ready to show us.

#### "Fork" the repository
Forking the repository is a way of making your own copy of it in your GitHub account. 
(Note: "repository" is the name for all the files making up the project).

````{tab} In the browser
If this is the first contribution you've made to the repository, then follow [these instructions](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository) to fork the repo for the first time. 
[This](https://github.com/very-good-science/our-handbook) is the repository that you want to fork.

If you've made a fork of the repository before, for an earlier contribution, then now you need to "sync" it, since your existing forked copy is probably a little out of date. 
To sync your fork, follow [these instructions](https://github.com/KirstieJane/STEMMRoleModels/wiki/Syncing-your-fork-to-the-original-repository-via-the-browser).
````

````{tab} Using your local machine
To get a copy of all the project files on your local machine you must first fork the repository (see instructions for 'In the browser') and then `git clone` **your fork** of the repository if you haven't already.

Cloning just means copying the project files to your local machine.
This repository that you need to clone will look like `github.com/YOUR-USER-NAME/our-handbook`.
[Here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) are some general instructions for cloning a repository, and [here]((https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)) shows an example of cloning a fork.

After cloning, open a terminal in the root of the our-handbook directory and install the necessary dependencies using `pip install -r requirements.txt`. You may first want to create a virtual environment.

If you already cloned the repository earlier, then you will instead need to checkout the main branch, and pull the latest changes from your newly synced fork. You may also need to install any updated dependencies using `pip install -U -r requirements.txt` inside your virtual environment.
````

### 4. Create a draft pull request
A pull request tells us where to look for changes you are making.

If you are working locally, then you may want to create a new branch before creating the Pull Request.

Creating a __draft__ pull request is really helpful to do up front because it shows us what is actively being worked on, and it also helps you get feedback.
You can follow [these instructions](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) to create the Pull Request. 
You will want to create a Pull Request from your forked repository to the `develop` branch of the `Our Handbook` repository.
Please fill out our Pull Request template as best you can.
 
### 5. Make your changes
Now you're ready to make your changes. 
As you "commit" new changes to your forked repository, the draft Pull Request that you created will automatically update.

```{seealso}
`Our Handbook` is a [jupyter book](https://jupyterbook.org/) which means that all the content for the book is written in MyST Markdown: you can find a useful cheat sheet [here](https://jupyterbook.org/reference/cheatsheet.html).
```

````{tab} In the browser

1. Go to __your fork__ on GitHub `github.com/YOUR-USER-NAME/our-handbook`.
2. Find the file that you want to edit
    - Most files you will want to edit will be in `book/guide` or `book/template`.
    - If it doesn't exist, you can [create a new file](https://docs.github.com/en/repositories/working-with-files/managing-files/creating-new-files) make sure it has the file suffix `.md`.
3. Edit the file:
    - Click the pen symbol to open the file editor.
    - Make changes in MyST Markdown.
    - You can preview changes, which will show you the general size of headings, but they won't be able to show some of the fancier MyST roles and directives.
4. Save (i.e. "commit") regularly.
    - When you've made a change (even if small), scroll down to where it says "Commit changes", and type a short meaningful message describing the change you made. I recommend committing changes regularly (every 20 minutes or so).
    - Make sure "Commit directly to the `main` branch" is checked.
    - Click "Propose file change".
  
Repeat until you're happy!
````

````{tab} Using your local machine
1. Open the file that you want to edit in your favourite text editor. 
    - Website content is in either `book/guide` or `book/template`.
    - Create a new `.md` file if needed.
2. Edit the file
    - Make changes in MyST Markdown.
3. Build the site to check that it looks as you expected
    - To check how the site looks, go to the root of the repository and run: `jb build book/`
    - After completion, you can run `open book/_build/html/index.html` to view the website.
    - Please do this before you mark your PR as "Ready for Review".
4. Save, commit, and push to your fork regularly.
````

### 6. Tell us you're finished
It's the final step!
All that's left to do is to follow [these instructions](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/changing-the-stage-of-a-pull-request#marking-a-pull-request-as-ready-for-review) to mark the Pull Request that you made earlier as Ready for Review.

What happens next is that a member of the Our Handbook team will check your changes to make sure that we can bring them into the main repository.
At this time we're likely to start talking to you in the Pull Request, and hopefully your changes will soon be ready to merge in!
