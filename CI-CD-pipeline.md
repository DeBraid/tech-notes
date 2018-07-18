# CI/CD Pipeline

Continuous integration and deployment (CI/CD) is used in modern software development.  The following is rough notes on this topic:

## CI/CD Tools for Node.js

via https://nodesource.com/blog/seven-convenient-ci-cd-tools-for-your-node-js-projects/

> CI/CD takes a huge step in the direction of clean, maintainable, and production-ready code - it helps us spot errors, spend more time writing code, and less time fixing it.

* `Travis-CI`: CI system: simple to set up quickly and efficiently, paid for commercial projects
* `Jenkins`: self-hosted with broad scope, can be quick to setup, extensive plugin ecosystem, runs official Node.js CI server (runs build process for majority of official Node.js project, see https://ci.nodejs.org/)
* `CircleCI` and `CodeShip` are other SaaS/IaaS alternatives

### Tools for Node.js Builds in Your CI/CD Pipeline

* `Snyk`: vulnerability monitoring and prevention service, detects and deals with security issues with PR checks in GitHub, at build-time, or custom.
* `Greenkeeper` is an interesting tool that’s useful for ensuring your modules are up to date.
* `Danger` is a pretty awesome tool to help with detecting and resolving common issues in PRs.
* `Docker`: containerizing your Node.js app can generate some "easy" optimizations


# CIRCLE CI

* integrates with GitHub: Every time you commit code, CircleCI creates a build, can automatically tests your build in a clean container or virtual machine.
* get notified if a build fails so issues can be fixed quickly.
* Passing builds are deployed to various environments so your product goes to market faster.
* seems like containerization optimal usage, possibly required.


### Automate GitHub Releases with CircleCI
via https://circleci.com/blog/publishing-to-github-releases-via-circleci/

`Releases` is a GitHub feature that allows you to present significant snapshots of your code, marked with a git tag, in GitHub’s nice UI.  Its a github features layered on top of tags.

# JENKINS

via https://wiki.jenkins.io/display/JENKINS/NodeJS+Plugin

### Main features
* NodeJS auto-installer (create as many NodeJS installations "profiles" as you want)
* install globally some npm packages inside each installations, these npm packages will be made available to the PATH
* execute some NodeJS script, under a given NodeJS installation
* use custom NPM user configuration file defined with config-file-provider plugin to setup custom NPM settings

### React Node App with JENKINS

via https://jenkins.io/doc/tutorials/build-a-node-js-and-react-app-with-npm/

* A macOS, Linux or Windows machine with: 256 MB of RAM, 10 GB of drive space for Jenkins and your Docker images and containers.
* must install: `Docker` and `git`

Lots of detailed steps in this tutorial on how to execute build scripts with Docker+Jenkins.


# Dockerizing Node.js

via https://nodesource.com/blog/8-protips-to-start-killing-it-when-dockerizing-node-js

Containers are the best way to deploy Node.js applications to production. Containers provide a wide variety of benefits, from having the same environment in production and development to streamlining deploys for speed and size.

Link above contains some practical tips and code snippets on structuring a Docker file for optimal usage with node js.

```
One of the largest benefits of using Docker is the ability to run large portions of their infrastructure locally on development machines. When using Docker images for local development, there will be constant pressure to add developer tooling into the Docker images.

An easy way to get large wins from Docker is to keep images linear. This means when building Docker images for use in CI/CD, development, and so on, the production Docker image should be used as the base image, and any extra tooling should be added as layers on top.

The benefit of this inheritance model - where development images inherit the environment from the production image - is that all the tests, code coverage, and linting are being run in the same environment that will be pushed into production.

As a team increases its use of Docker, this practice ends up yielding a much better developer experience. When this pattern is used, bugs that manifest themselves in an application's production images will nearly always manifest themselves in the developer images as well.
```
