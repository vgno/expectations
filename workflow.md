# Expectations for Workflow

## Use the Version Control System

VCS are not stupid audit/archive tools. Learn them, learn them good, and use all
the features!

## Use Coding Standards

Follow our [Coding Standards](https://github.com/vgno/coding-standards) for the
language you develop in. If you disagree with the existing standard, use pull
requests to propose changes.

If you start using a language we do not have a Coding Standard for, propose one.

## Write Good Commit Messages

Read and follow [Commit Message Standards](workflow/commit-messages.md) document.

## Have a clean branch that is always deployable

If ops need to fix a critical bug during the weekend, they need to be sure they
are deploying the hotfix and not 10 other things at the same time. Suggested
practice is to follow [Gitflow](http://danielkummer.github.io/git-flow-cheatsheet/),
[Github flow](https://guides.github.com/introduction/flow/), or other practices
that keep one branch deployable.

## Use Feature Branches

Any feature or change should be done in feature branches. Commit small, push
often.

If you follow git flow, suggested naming convention is to have:

  - master
  - develop
  - feature/* (e.g. feature/new-gallery-widget)
  - release/* (e.g. release/1.2)
  - hotfix/* (e.g. hotfix/1.2.1)

## Leave Code Better than You Found It

If you can't fix it at the moment, always create issues, tickets or markers so
someone can pick it up later. Smelly code should never be discovered twice.
