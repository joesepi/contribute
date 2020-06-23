# The OpenJS New Contributor’s SCRIPT


## Outline

1. Intro
1. Preface
1. Etiquette (new/maintainers)
1. Community Health view (COC first)
	1. Code of Conduct
	1. Contributing
	1. License
1. /contribute
	1. good first issues ++
	1. doc and other issues; doc is good place to start
	1. link to contributing
1. Processes
1. Prereqs
1. Github OSS contributing flow
1. Contributing doesn't always mean code
1. OSS on company time
1. Other resources
1. Open Office Hours

## Intro

Hi. Its me. What do I do

- IBM
- Node.js community
- OpenJS Foundation

## Preface

preface, prelude, etc

we will center our journey here today around new contributors but we will weave in wisdoms for maintainers and more experienced contributors

## Etiquette and frame of mind - contributors

- daunting; me too; dip your toe in
- be courteous; ask questions; assume good intentions
- read contributing guidelines; follow procedures and guidelines
- be open to constructive criticism; code will be reviewed but remember to assume good intentions; learn from doing

## Etiquette and frame of mind - maintainers

- daunted
- be courteous; no dumb questions; assume good intentions
- be sure contributing guidelines and expectations are clearly documented
- be constructive in critiques; remember to assume good intentions, see also daunted comment

## Community Health

- Check community health of a project
	- examine for CoC !!!!!
	- Contributing guidelines
	- license

Note: maintainers check how your project looks

## `/contribute`

- github.com/nodejs/node/contribute
- gfi and other changes that github algorhythmically determines is good entry points
- link to contributing again

Note: maintainers check how your project looks

## Processes

- Contributing guidelines
- Git commit message guidance
- Code style guide
- Doc style guide

From Node Contributing:
If you are new to contributing to Node.js, please try to do your best at conforming to these guidelines, but do not worry if you get something wrong. One of the existing contributors will help get things situated and the contributor landing the Pull Request will ensure that everything follows the project guidelines.
 
## Prereqs

Some projects have prerequisites and dependencies and even underlying tooling that you may need to be aware of.

Node has some
ESLint is another good example (AST understanding)

## Github OSS contributing flow

Fork the project on GitHub and clone your fork locally.

```
$ git clone git@github.com:username/node.git
$ cd node
$ git remote add upstream https://github.com/nodejs/node.git
$ git fetch upstream
```

#### Configure git if necessary
```
$ git config user.name "J. Random User"
$ git config user.email "j.random.user@example.com"
```

#### Branch from Main

As a best practice to keep your development environment as organized as possible, create local branches to work within. These should also be created directly off of the master branch.

```
$ git checkout -b my-branch -t upstream/master
```

#### Do the work

Make changes, and when changes are ready make sure you run tests and any linting or style checkers, then:

```
git add your/files or .
git commit
git push origin your-branch
```

If your work needs updates from upstream, remember, rebase is your friend.

```
$ git fetch --all
$ git rebase upstream/master
$ git push --force-with-lease origin my-branch
```

Note that `force` rewrites history. It can be dangerous if not used correctly.

#### Rebase is your friend

As a best practice, once you have committed your changes, it is a good idea to use git rebase (not git merge) to synchronize your work with the main repository.

```
$ git fetch upstream
$ git rebase upstream/master
```

This ensures that your working branch has the latest changes from nodejs/node master.

## Contributing doesn't always mean code

There are a number of ways you can contribute to a project without writing core source code.

#### General
- docs
- website
- project management
- social/community/outreach

#### Other projects
- Node-RED nodes
- Loopback datasource connectors

#### Node
- Release team
- Build working group
- website
- i18n
- social/community/outreach
- examples

Note: mention COLLAB SUMMIT

## OSS on company time

- Open Source Fridays
- My experience at Adobe/Behance

## Other resources

- https://github.com/showcases/great-for-new-contributors
- https://opensource.guide/how-to-contribute/
- https://www.firsttimersonly.com/

## Open Office Hours
 
 https://github.com/openjs-foundation/open-office-hours
 

---

## BAK

Notes:

when narrating and expecting some code in terminal say "just tap tap tap ..and bing"

talk as if you are showng. verbal vanna white. riff ready.

test future self by oretending a hologram effect snd see ig future self figures out how to make it work. 

## Talk Description

https://sched.co/bwCK

Based on conversations and interviews with a variety of collaborators and maintainers from a number of open-source projects, we'll explore the ways in which you can become a valuable contributor to a project and its community. If you're new to open-source, we'll touch on how to get started, best practices, where to look for help and how to identify good communities. If you are already involved, we'll discuss how to make your environment more welcoming and how you can help new folks be successful. We'll focus on a number of OpenJS projects including Node.js and its many teams and working groups (Releases, Package Maintenance, Security, Modules, etc.), but the takeaways can apply to any open-source project. We'll even spend a moment on open-governance and how foundations work. It'll be fun!
