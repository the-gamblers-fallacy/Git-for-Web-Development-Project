# Setting Up Your Computer

Welcome to day 1 at BloomTech, today we are going to spend time setting up your computer and learning the tools that you will be using to complete this program. Just like day 1 at a job, you will need to get your environment set up to build and run your code. Complete the set up tasks below and then get started on the research questions. Once you have finished check out the submission instructions in the `README.md` file to turn in your assignment for the day. 

## Set Up Tasks 
1. [x] [Download xcode](https://apps.apple.com/us/app/xcode/id497799835?mt=12) - these are your developer tools for mac 
2. [x] sign up for a [GitHub account](https://github.com/join) - please use a professional username. We recommending using your `firstname` `lastname`
3. [x] [Set up your SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) - GitHub uses SSH to keep their files secure. You will need to set up one SSH key for every computer that you want to access your GitHub account on. Please ensure you go through all of the steps to generate a new key, add a new key and test your connection.
4. [x] [Download Zoom](https://zoom.us/download) - make sure your zoom display name is your `first name` `last name`
5. [x] [Download Slack](https://slack.com/help/articles/207677868-Download-Slack-for-Mac) - make sure your slack display name is your `first name` `last name` 
6. [x] [Download VS code](https://code.visualstudio.com/download) - this will be the tool you use to write all of your code. We recommend installing the following extensions: 
- [ES Lint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
- [Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
- [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
7. [x] [Download Node.JS](https://nodejs.org/en/) - Please download the latest stable version. We will be using Node.JS to run the tests in all of our javaScript assignments. Test driven development is a common practice in the world of web dev. You can read more about it [here](https://www.freecodecamp.org/news/test-driven-development-what-it-is-and-what-it-is-not-41fa6bca02a2/) 
8. [x] Sign up for a free [codepen account](https://codepen.io/accounts/signup/user/free)
9. [x] Sign up for a free account on [Lucid Chart](https://www.lucidchart.com/pages/landing?utm_source=google&utm_medium=cpc&utm_campaign[…]tTwOoXp_lCeLTC97pikTFa5cE58FWHwjjpTSGsGPRqR2AAaAh-MEALw_wcB)

## Research Questions 

Now that you are all set up, it's time to learn a little more about the tools of the trade. Edit this file and answer the following questions. You can type your answer below the questions. You are going to need to start familiarizing yourself with the [GitHub docs](https://docs.github.com/en) doc short for documentation are the instructions on how to use a languge, or program. A large part of your job as a developer will be learning how to read and work with documentation. Please reference the GitHub docs when answering the questions below. If you cannot find what you are looking for in the docs, you can always start to practice your google skills. 

1. What is git? What is the difference between git and GitHub?

Git is a version control language that allows you to keep track of changes made to code, and revert and see those changes in a variety of ways. Github is a manager for your git repositories, and allows you to store your repositories online, share them with others, and collaborate on changes.

2. Why do we create a branch? 

Rather than working on the 'main' branch, we make branches to make changes without risking breaking our 'source of truth' for our code. If something breaks on a branch, that's no big deal. If something breaks on 'main', it might mean it breaks for other people when they fork your repository, and navigating to previous versions becomes trickier.

3. What is the purpose of a pull request? 

A pull request is sort of a fail safe between a developer and the 'main' branch. It allows you and other developers to see changes made, as well as hopefully identify any issues before a branch is merged into the main that everyone's working on. Also, they allow other devs to checkout your pull request and test it out to make sure it's working.

4. What is the command you can use to switch between branches? For example you are working on a feature branch and you want to switch back to main. 

`git checkout <branch_name>`

5. Explain the difference between `git fetch`, `git merge` and `git pull` what does each command do? 

`git fetch` is a way to get changes made on a remote branch locally without goofing anything on your end. A fetch won't attempt to "merge" the remote repository code into your local repository. `git pull` also gets changes made on a remote branch, but will then attempt to stuff those changes into your code locally. If you have changes that conflict with someone else's, you'll have to choose which one to keep and then it can get messy! `git merge` is somewhat similar, except it's done when you want to combine two branches into one. If you have a branch you want to put into main, you'd merge, and provided there are no conflicts, the main will then have the changes made on the branch, and the branch can be safely deleted.

6. What is a merge conflict? How do you resolve a merge conflict? 

A merge conflict arises when git attempts to combine code somehow, through a pull or a merge, and finds disagreeing changes between the combining pieces. For instance, if you and your dev friend didn't communicate and both changed the `<h1>` tag in your index.html file to read two different things, git would get mad at you both. At this point, one of you has to figure out which change you are going to keep, commit the change to prevent a conflict, and then attempt the merge again.
