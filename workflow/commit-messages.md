# Commit Message Standards

This document describes how commit messages should be written, formatted, and what they should contain.

(IMPORTANT) It should **by the 50 character summary alone** be possible to understand what code the commit affects.

## Example Commit Message

```Capitalized, short (50 chars or less) summary

More detailed explanatory text, if necessary.  Wrap it to about 72
characters or so.  In some contexts, the first line is treated as the
subject of an email and the rest of the text as the body.  The blank
line separating the summary from the body is critical (unless you omit
the body entirely); tools like rebase can get confused if you run the
two together.

Write your commit message in the imperative: "Fix bug" and not "Fixed bug"
or "Fixes bug."  This convention matches up with commit messages generated
by commands like git merge and git revert.

Further paragraphs come after blank lines.

  - Bullet points are okay, too

  - Typically a hyphen or asterisk is used for the bullet, followed by a
    single space, with blank lines in between, but conventions vary here

  - Use a hanging indent

Close T123
Fix T123
Resolve T123
Reference T321```

# Formatting Rules

  - Subject should not be longer than 50 chars.
  - Subject should not end in a punctuation.
  - Subject should always be separated from the body with an empty newline.
  - Body should be wrapped at 72 chars.

# Content Rules

All commits MUST have:
  - A Subject Line which clearly and shortly describes what's being changed in the commit.

All commits SHOULD have (when necessary):
  - A Body describing what, how and why the change is being done if this is not clearly summarized in the Subject Line.

If the commit is relevant to a issue, the issue should be referred as well.

## Subject Line

Subjects should be written in [[ http://en.wikipedia.org/wiki/Imperative_mood | imperative mood ]] which means "spoken or written as if giving a command or instruction".

A properly formed git commit subject line should always be able to complete the following sentence:

> If applied, this commit will **your subject line here**

  - If applied, this commit will **refactor subsystem X for readability**
  - If applied, this commit will **update getting started documentation**
  - If applied, this commit will **remove deprecated methods**
  - If applied, this commit will **release version 1.0.0**
  - If applied, this commit will **merge pull request #123 from user/branch**

IMPORTANT: Notice how this doesn't work for the other non-imperative forms:

  - If applied, this commit will **fixed bug with Y**
  - If applied, this commit will **changing behavior of X**
  - If applied, this commit will **more fixes for broken stuff**
  - If applied, this commit will **sweet new API methods**

## Body

The commit body should also be written in the imperative form.

  - Include information about why the change is being done (who/what caused the change to be done).
  - Include any background information that will be useful.
  - Add references to relevant issues and commits [with the GitHub Reference Notation](https://help.github.com/articles/writing-on-github/#references)
