```
Roberto Nogueira  BSd EE, MSd CE
Solution Integrator Experienced - Certified by Ericsson
SkypeID: enogrob2005
Email  : enogrob@gmail.com
Profile: http://www.linkedin.com/in/enogrob
```

# Rails App Reddit

![reddit logo](app/assets/images/reddit.png)

## Features

* Sign up / Sign in & Out
* Submit a link with a Title & URL
* Vote up or down on a link
* Comment on links submissions

## Steps performed

### Rvm preparation

```bash
$ rvm install 2.1.1
$ rvm gemset create rails-4.1.5
$ rvm use ruby-2.1.1@rails-4.1.5
$ rvm --ruby-version use ruby-2.1.1@rails-4.1.5
$ gem install rails --version '4.1.5'
```

### Create new Rails application

```bash
$ rails new TRailsApp_reddit
$ cd TRailsApp_reddit
```

### Initialize Git

```bash
$ git init
$ git status
$ echo .idea >> .gitignore
$ git add .
$ git commit -m "First Commit"
$ git create TRailsApp_reddit
$ git push origin master
$ git browse .
```
