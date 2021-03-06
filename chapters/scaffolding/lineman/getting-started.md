# Getting started

## Installation

Lineman is a Node.js-based tool, and it requires `npm` to install it.

Lineman is installed globally:

```bash
npm install -g lineman
```

You can test it by running:

```bash
lineman --version
```

## Creating a project

To create a new lineman project, just run:

```bash
lineman new some-project-name
```

This will create a project in `some-project-name/` with a small scaffold of directories and files. It'll include several safe-to-delete example files. Once you're comfortable, you may want to generate the project again with the "--skip-examples" flag to start completely fresh.

## Developing

Once you've changed into your project directory, you can see your app in action by running:

``` bash
lineman run
```

This will do an initial build of the application into a transient folder named "generated/" and start a local server out of that directory. You can access it at [localhost:8000](http://localhost:8000).

The `run` command also watches for file changes, re-running any appropriate tasks. It also exposes powerful API proxying and stubbing tools that let you develop your web application in concert with other backend services (whether or not they actually exist yet).

## Building

When you're ready to deploy, run:

``` bash
lineman build
```

And this will build a ready-to-deploy set of artifacts in a directory named "dist/". By default, this means minifying your scripts & stylsheets.

## Configuration

TODO: configuring asset fingerprinting

TODO: Setting up an API proxy

TODO: API Stubbing

TODO: deploying to heroku

TODO: Ruby on Rails integration

TODO: using Lineman plugins
