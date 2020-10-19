# Markdown

## Objectives

* Create your own Markdown profile page
* Understand the GitHub workflow (including commits, and pull requests)

## Preparation

[Markdown](https://en.wikipedia.org/wiki/Markdown) – a lightweight markup language with plain text formatting syntax.

[MDwiki](http://dynalon.github.io/mdwiki/#!quickstart.md) – a CMS/Wiki built in HTML5/Javascript and runs on the client. It uses Markdown as its input markup language. The website you are currently viewing is realized with MDwiki.

### Markdown
The following resources can be used (and bookmarked) to familiarize yourself with Markdown:

- [GitHub – Mastering Markdown](https://guides.github.com/features/mastering-markdown/) - The official GitHub Guide for Markdown syntax.

- [Markdown cheat sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) - A bigger Markdown cheat sheet with examples.

- [Markdown Tutorial](https://tylingsoft.github.io/tutorial.md/#whats-markdown) - An interactive tutorial to learn Markdown.

- [Markdown Interactive Tutorial](http://www.markdowntutorial.com/lesson/1/) - Another awesome interactive tutorial to experiment and learn more Markdown syntax.

**NOTE**:
• **If you have not used Markdown before, we recommend you to go through at least one of the tutorials/guides.**


## Start Here

Below is a summary of the steps that we will walk you through:

* [Create a new file as your personal MDwiki page and commit your changes](#Create_a_new_file_as_your_personal_MDwiki_page_and_commit_your_changes)
* [Open a pull request](#Open_a_pull_request)

### Create a new file as your personal MDwiki page and commit your changes

**Again, when you're editing on GitHub, it is important to make sure you are working on your own GitHub repository.** To that end, make sure there is your own username before the slash and the correct repository after the slash. For example: `EmilyLarkin/EmilyLarkin.github.io`.

First, before creating your file, we need to create a new branch

1. Click on the branch selector menu (make sure it says "Branch: **master**", if it's something else, click on it and switch to master branch first
1. Give your new branch a short and descriptive name (you can read more about branch naming [here](https://github.com/agis/git-style-guide#branches))
1. Click on "Create branch: your-new-branch-name". Then you should see "Branch: **your-new-branch-name**" on the branch selector menu

Next, we are going to create your page

1. Go to the `pages/micromaster/profiles` folder
1. Make sure you are still on the new branch you just created, look for "Branch: **new-branch-name**" on the branch selector menu
1. Click `Create new file` button
1. Name the file exactly the same as your GitHub username plus the `.md` file extension `<username>.md`
  * It is important that you stick with your GitHub username so we could easily identify you


Then, in the new Markdown file, include the following information:

* your name, location/time zone, and OS (including version)
* a short description of yourself (so your fellow virtual interns know who you are)

You may use the "Preview" tab to have a primitive look of what your Markdown will look like. Please use at least 5 different types of Markdown elements so you can get an idea of how it works. Avoid using HTML as the purpose of Markdown is to make pages easy to write and read. Try to be as creative as possible.

When you are finished, press 'commit changes' below.


If you need to edit your file again, click the pencil icon to edit.

Now, check what this looks like on your own page `https://raw.githack.com/YourUserName/YourUserName.github.io/YourBranchName/#!pages/micromaster/profiles/YourUserName.md`. The [raw.githack](https://raw.githack.com/) link allows reviewers to preview your changes. Don't forget to add `#!` after the forward slash proceeding your branch name in order to show the markdown in presentation mode. Please double check that everything looks good and is working as you hoped before moving on to next section.

**NOTE**:
• If you don't see any changes in your page after editing your file then you need to clear your browser's cache or open your page in your browser's **"incognito"** or **"privacy"** mode. You can also press Ctrl+Shift+R or Ctrl+F5 to reload the page with cache cleared.
• As MDwiki site is what we use for "production," please **always check** if everything renders as you expected using raw.githack link. There are [different flavors of Markdown](https://github.com/commonmark/CommonMark/wiki/Markdown-Flavors). Use GitHub's preview tab for reference only.
• The [raw.githack](https://raw.githack.com/) link is different from the raw link available on Github page.


### Open a pull request

Once you have your profile ready, it's time to create a pull request. Click on one of the "Pull request" button.

**There are a few things to watch out before clicking on the green "Create pull request" button**. Make sure you:

* give the pull request a short and descriptive title (e.g. create YourUserName.md)
* include the raw.githack link to your Markdown profile page in the pull request description
* scroll down the page and verify you used at least 5 **different** Markdown elements in your profile

Finally, click "Create pull request" button and post the link to your github.io and profile pull request in the [slack chat](http://slack.ole.org):

> @/all I'm on step 3 - GitHub and Markdown, please look at `https://YourUserName.github.io` and review my profile pull request `LinkToYourPullRequest`

Remember, it can take a while for `https://YourUserName.github.io` to be up and running, so don't worry if you see a **404** when you access the link!


Someone from our team will review the changes and notify you on gitter. Often there will be some feedback from the reviewer for you to address. If that is the case, go to your pull request first then select "files changed" --> next select "..." on the top right --> select "Edit File" --> make the required changes --> scroll down and select "commit" on the pull request when done. Any changes you make to your branch will be automatically updated in the pull request. Once you get 2 approving reviews, we will merge your Markdown profile with the main repository.

After the pull request is merged, you'll be able to see your personal page at `planetlearning.github.io/#!pages/micromaster/profiles/<YourUserName>.md`. Let us know in the [slack chat](http://slack.ole.org)  after you complete this step.

**NOTE**: Try to add and experiment with as many markdown elements as you can and make your page attractive. Be creative.
