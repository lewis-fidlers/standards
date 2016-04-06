# 10to1 Standards

A collection of things we reuse in a lot of projects.

## Scripts

A set of scripts we use for ci, and getting team members up and running with a project.

These are just starter scripts that can be used to have a starter for a new project.

Loosely based on [Github's scripts to rule them all](https://github.com/github/scripts-to-rule-them-all/)

## [bootstrap](https://github.com/10to1/standards/blob/master/script/bootstrap)

Team members can run this script to get going:
it will install the bundle and tell the user which dependencies to install from their favourite package manager.

The script will also create database users, create some data in the DB, and any other configuration that is needed to run the project.

At the end of the script should output an explanation of how to run & use the app.

## [cibuild](https://github.com/10to1/standards/blob/master/script/cibuild)

Our ci uses this script to run whatever is needed to validate the project: Run the tests, check styleguides.

## Style guides

In this repo we'll also add the code style configuration that is used by our CI by default.

The CI uses [pronto](https://github.com/mmozuras/pronto) to validate conforming to the styleguide.

### The ruby styleguide

You can use the ruby styleguide as a base by adding it to your homedirectory

```
curl -Lo ~/.rubocop.yml https://raw.githubusercontent.com/10to1/styleguides/master/guides/ruby.yml
```

In our case this is installed for the CI-user. But can be overridden on a per project basis.
If a pull requests gets merged, don't forget to update style guides on ci if required.
