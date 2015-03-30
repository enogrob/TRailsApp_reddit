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

### Link Submissions
To have the ability to submit a link, we are going to generate a scaffold for our Links. Lets do that now. First lets create a new branch in Git.

```bash
$ git checkout -b link_scaffold
```

Then lets generate the Link scaffold:

```bash
$ rails generate scaffold Link title:string url:string
```

Now we need to migrate our database… So run the following:

```bash
rake db:migrate
```

Now we can visit <http://localhost:3000/links>, and you can see we have the ability to now add a new link, as well as edit & destroy the links. Generating the scaffold creating a bunch of files for us, including our model, view and controller files, as well as edited our routes. Which gives us the ability to add / view / edit / destroy links.
Everything is looking good so far, so lets commit & merge what we just did.

```bash
rails server
```

Everything is looking good so far, so lets commit & merge what we just did.

```bash
$ git status
$ git add .
$ git commit -am "Generate Link Scaffold"
$ git checkout master
$ git merge link_scaffold
$ git push
$ git browse .
```


