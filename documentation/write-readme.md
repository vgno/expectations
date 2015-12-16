# README.md

All repositories MUST have README.md in the root. This file should contain information about:

  - A brief description of the repository
  - Instructions on how to set it up (which build tool target to execute)
  - Instructions on how to run tests
  - Instructions on how to deploy

## Example README.md

  lang=text, name=README.md

  # Example Project

  **Short** description of the Example Project.

  ## Documentation

  Include any references to documentation related to the project. Add links
  to Wikis, Google Docs, and/or any other resource.

  ## How to Build

  This must be all the steps necessary to get the application up and running
  from a fresh checkout.

  It should be automated with either Rake, Ant, Gulp, Grunt, Make, Npm,
  Composer or similiar.

  ``` sh
  make install
  ```

  ## How to Test

  Running the testsuite should be automated.

  ``` sh
  make test
  ```

  ## How to Deploy

  A good idea is to also include how to list all the available deploy targets.

  If the application has no automated deployment, write all the steps required
  to do it manually.

  ``` sh
  make deploy TARGET=production
  ```
