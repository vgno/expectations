# Automate Building

Automated building is every step required to have a runnable application.

This typically includes:
  - Installation of dependencies
  - Compiling and preparation of assets (CSS, JS, GFX, etc)
  - Setting up folders and permissions required for run-time

Each steps in an automated build is usually achieved by several specific tools, orchestrated by one generic build system.

## Build Systems

Build Systems are generic and can be used for automating several specific steps.

### Common Build Systems

Name       | Description
---------- | ---------------
Bash       | Any shell script.
Apache Ant | Java based task runner.
Phing      | PHP based version of Ant. Installable with Composer.
Make       | Standard goto tool for Unix.
Rake       | Make-like tool based on Ruby.
Gulp       | Node based build tool with focus on streams. Installable with NPM.
Grunt      | Node based task runner. Installable with NPM.
