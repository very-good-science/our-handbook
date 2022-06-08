# What to do during a workshop

```{note}
This page will guide you through what will happen on the day of your workshop.
The person organising the workshop should complete the steps on the [before a workshop](./before-a-workshop.md) page,
including forking this template to your own GitHub organisation.
```

During a workshop, you can expect to:

- Decide what you're going to work on
- Spend some time working on your tasks#
- Ask facilitators for help at any time!

## Decide what you're going to work on

Discuss in your group and agree what content and sections should be in your finished handbook.

Create issues for each of these, containing suggested tasks.

Decide on rough priorities (e.g. “must-have”, “nice-to-have”, "long-term-goal").

Assign each person a first task.

## Spend some time working on your tasks

In this workshop, we suggest that work is split up into multiple 25 minute bursts, where you
can work on tasks which have chosen to do, or which have been assigned 
to you by your team. The task will likely involve changes to your groups handbook, each
change can be broken down into the following stages:

1. Making a copy (fork) of your organisations handbook
2. Editing some part of the handbook 
3. Inserting the changes (via pull request) back into your organisations handbook

```{tip}
Breaking your work into these small chunks is called
the "Pomodoro" technique. You can use a [pomodoro timer](https://pomofocus.io/)
to time your teams work on their tasks.
```

### Making a Fork of Your Organizations Handbook

Usually, it is best not to make changes directly to your 
organisations handbook. This can make it difficult for others who
are making changes, and it is also better to give other members 
of your team a chance to check your work before it is merged. 
This is why you should work off of your own "fork".

To fork your organisations repository, go to your organisation's
handbook page, and click the `fork` button. See [here](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
for more detailed instructions, and further explanations of forks.


### Editing Pages

All of the pages that make up your handbooks are markdown files.
Markdown files are simply textfiles with the extension `md`, they 
have a few extra features which you can learn about [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax). To edit pages
you can go to the markdown and edit the text file. 

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
[Here](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) are some general instructions for cloning a repository, and [here]((https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)) shows an example of cloning a fork.
```
````


````{note}

It is important you know how to find the correct file to edit. 
On the left of this page you can see a side bar with the handbook layout.
If you wanted to edit this page, you would need to find the file of the 
"What to do during a workshop" page. The repository structure looks something
like this:


```
📁 OUR-HANDBOOK
|
├ 📁 book
| |
| ├ 📄 _config.yml
| |
| ├ 📄 _toc.yml
| | 
| └ 📁 guide
|   |
|   ├ 📄 what-is-our-handbook.md
|   ...
├ README.md
...
```

The `_toc.yml` file can give you an idea of what the structure of
the site is. For example, the `_toc.yml` for this page looks 
like this:

```
format: jb-book
root: guide/what-is-our-handbook
parts:
  - caption: User Guide
    chapters:
    - file: guide/how-to-use/how-to-use-overview
      title: How to use this template
      sections:
      - file: guide/how-to-use/editing-together
      - file: guide/how-to-use/put-online
      - file: guide/how-to-use/during-a-workshop
```

Based on this, you can see that you would need to edit the 
`guide/hoe-to-use/during-a-workshop.md` file. This is also
why it is helpful to use informative file names!
````

### Saving Changes

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

### Merging Changes

A _pull request_ tells your group where to look for changes you are making.
You can wait until all your changes are made before creating your pull request, but it is really helpful if you create one as soon as you start making changes.
Creating a __draft__ pull request up front shows us what is actively being worked on, and it also helps you get feedback early into making your changes.
When you add more commits, your draft pull request will automatically update.

- Create a pull request from your forked repository to the `main` branch of your organisations handbook repository
- We recommend you create a __draft__ pull request as early as possible
- Please fill out our Pull Request template as best you can

```{seealso}
You can follow [these instructions](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) to create the Pull Request. 
```

### 6. Tell your team you're finished
It's the final step!
All that's left to do is [mark your pull request as ready to review](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/changing-the-stage-of-a-pull-request#marking-a-pull-request-as-ready-for-review).

A member of your organsiation will check your changes to make sure that you can bring them into the main repository.
At this time you should start talking by leaving comments on your pull request, and hopefully your changes will soon be ready to merge in!



