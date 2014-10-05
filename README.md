# Liberator

> The official tool you'll use to publish the work you've done (during sprints) at Hack Reactor.

## Table of Contents

- [Overview](#overview)
- [Guidelines](#guidelines)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
  - [All At Once](#all-at-once)
  - [One by One](#one-by-one)
    - [Single Repo](#single-repo)
    - [Multiple Repos](#multiple-repos)
  - [Eligble Repos](#eligble-repos)

## Overview

Liberator publishes your Hack Reactor sprint repositories, doing the following in the process:
- Fixes your repositories' git history so that you get full credit for all commits made by the `hackreactor-students` account on a Hack Reactor workstations (This fills in your GitHub commit history in the process.)
- Adds a basic readme explaining to the world what this repository is.
  - NOTE: This will delete any existing readme.md file in the repo.
- Deletes your old, private repository.
- Publishes your private sprint repository as a public repository.
- Deletes all branches except 'master' 
  - You probably don't want a potential employer comparing your code with a branch on your repo labeled 'solution' :D

## Guidelines

- **DO** publish any repository you did any work on, even if it's incomplete or
  sloppy by your current high standards. Employers will see these repositories
  will care about one thing: that you've been writing code for three solid
  months.
- **DO NOT** publish any curriculum outside of (or otherwise circumvent)
  Liberator. Hack Reactor's curriculum represents thousands of hours of work put in by many different individuals, and not all of it is public domain.
  (Curriculum does not, of course, include personal projects, group projects,
  etc. Those should be public already, unless the particular constraints of your project dictated that it be private.)
- **DO** publish your repositories before graduating. You don't have to publish your sprints in 'real time' if you don't want to. You're welcome to publish them all at once during the second half of the course instead. Just know that Hack Reactor will delete your cohort's
  master curriculum repositories twelve weeks after your graduation. If you do
  not publicize your repositories before then, your work will be lost forever.

## Installation

__NOTE__: You do not need to fork this repo to install/use the liberator tool.

Run the following (you'll be prompted for you github username and password):

  ```sh
  npm install -g git+https://github.com/hackreactor/liberator.git
  ```

## Configuration

The first time you run use the tool via `liberator`, you will be prompted for your github email, github username, and github password. The tool uses these to generate an OAuth token that is saved locally and used for all subsequent requests.
  - NOTE: You must use the e-mail that you use on GitHub. It determines what is counted as _your_ commit, so make sure it is right.

## Usage

### All At Once

If you want to liberate _all_ of your eligible repositories (see below), run `liberator all`

### One By One

You can also liberate them one at a time (or a few at a time), by listing the repositories in a space-separated list after the tool:

#### Single Repo

`liberator 2014-04-databases`

#### Multiple Repos

`liberator 2014-04-chatterbox-client 2014-04-chatterbox-server` will also work

### Eligble Repos

Liberator will only work on the following repos (whether run with the 'all' flag or individually):
- blackjack
- chatterbox-client
- chatterbox-server
- data-structures
- databases
- javascript-koans
- looper
- middleware
- mvp
- mytunes
- n-queens
- oath
- recursion
- shortly-angular
- shortly-deploy
- shortly-express
- subclass-dance-party
- taxonomy
- timecop
- twittler
- underbar
- watchout
- web-historian
