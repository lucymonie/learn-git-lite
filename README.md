# Git for non-technical members of a tech team

If you're a member of a tech team but your function is non-technical, it is useful to know how to use git and Github as this is a key tool for technical team members. Having git installed on your machine and being able to pull down code and run it locally will likely come in useful.

## What is git?
Git is a version control system. Version control systems are software that help you track changes you make in your code over time. As you change your code, you instruct the version control system to take a snapshot of your files (these are called commits). The version control system saves that snapshot permanently so you can recall it later if you need it.

Without version control, you may be tempted to keep multiple copies of your code. It’s easy to change or delete the wrong file, potentially losing work. Version control systems manage all versions of your code but present you with a single version at a time (usually the latest).

## Your OS
This tutorial assumes you are on a Mac.

## Install iTerm2 and Homebrew
Download iTerm2: https://www.iterm2.com/
Start by installing homebrew: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
Then `brew update`

## Install atom
Atom is a text editor suitable for code: https://atom.io/
You'll need this sometimes to open up and run the code, though most of commands are entered in the terminal.

## Install git
Open your terminal and run `brew install git`

## Create a notes repository
- Open a browser window and go to your github account homepage (https://github.com/[username])
- Click on menu item `repositories`
- Click the green buttons `New`
- Call your repository `notes`
- Click the green button `Create repository`


## Clone your repository
- In the section `Quick setup`, click on the `https` button, then click on the `copy to clipboard` arrow button on the far right
- Switch to your terminal
- Enter `cd Documents` in the terminal
- Enter `git clone ` and then paste in the link to your repository that you copied a minute ago
- Enter `cd notes`
- Enter `atom .`

## Create a file
- Make a new .md file which is good for writing notes.
- Save it.

## Push it up to github
- Go to the terminal
- Type `git status` (should should see the name of the file you just added, marked `untracked`)
- Type `git add ` plus the name of the file you just added
- Type `git commit -m ` plus a commit message in quotation marks. This should say why you are adding this information.
- Type `git push origin master`
- Enter your git username and password when prompted.

## View it on github
- Go back to github and you'll see the file you just pushed up has appeared.
