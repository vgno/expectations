# Expectations for Documentation

Documentation can be broken in to two main categories, one for the code itself,
and another for the surrounding project.

When the "distance" between code and documentation is far, it provides less
value (nobody finds it), and increases the probability for it not being
maintained together with the code.

## [Write a README.md](/documentation/write-readme.md)

All repositories MUST have README.md in the root. This file should contain
information about:

  - A brief description of the repository
  - Instructions on how to set it up (which build tool target to execute)
  - Instructions on how to deploy

## Write Self-documenting Code

The code should be self-documenting and not rely on additional documentation to
be read and understood.

## Write Wiki for non-developer documentation

Wikis should only be used for surrounding documentation, for example end-user
docs.

## API documentation

External facing APIs should be documented as close to the code as possible. This
means inline with comments or annotations, or in a separate files in the same
repository. Typical examples is phpDocumentor (docblocks) for shared libraries
and Swagger for HTTP APIs.
