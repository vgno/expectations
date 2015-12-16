# Expectations for Automation

Humans make mistakes, machines do not. Repetitive tasks should always be
automated.

## [Automate Building](/automation/building.md)

Use ant/rake/make/grunt/gulp or any other build tool to automate any build steps
required for the Applications. Chosen tool has to be able to setup any of
the environments (development, staging, production etc.) and not only prod for
example.

## Automate Deployment

Neither frontends or backends should be deployed manually. An automated approach
MUST be used. Typically this would be [Capistrano](http://capistranorb.com/) or
[Deployer](http://deployer.org/).

IMPORTANT: Deployment MUST be separated from building.

## Automate Regression Testing

Both frontends and backends should include one or more testsuites which,
depending on the size and importance of the application, should range from unit
tests, integration tests, functional tests to acceptance tests. If you need help
understanding the difference between kinds of tests, please read
[The Grumpy Programmer's PHPUnit Cookbook](https://leanpub.com/grumpy-phpunit).

## Automate Code Metrics

Code metric collection should be exerted on both the frontend and backend
codebases. This is typically lines of code, test coverage, copy-paste detectors,
complexity analysis, etc. Thresholds for marking the build unstable / failing
should be set to the level agreed by the team (until they are agreed commonly)
e.g. 'if coverage went down by more than 5% in the last build, mark it unstable'.

## Use Continuous Integration

The regression tests and code metrics collection should always be ran
automatically on post-commit by an Integration server. A good practice is to
have separate jobs for unit tests (builds fast), integration (triggered after
success of unit tests), any other tests.
