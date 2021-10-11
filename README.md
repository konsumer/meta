# github meta

Here I will track my process of getting all my github projects in order.

## general goals

- Categorize all projects "supported" or "unsupported"
- edit README, npm depracate, and archive any unsupported project
- Use [topics](https://github.com/topics) to tag projects
- try to automate all steps below with github bots or actions

## org categories

Things should be better categorized by what they are for.

- konsumer - my own libraries, things published on docker/npm, etc
- notnullgames - game (or hacking) libraries/demos


## project types

### node web library

These are projects that only function as a library for a web project.

<!-- put list here -->

They should have these setup:

- issue templates
- docs for API (either in README.md or API.md)
- update/audit all dependency packages regularly
- installation instructions
- es6 + microbundle
- FUNDING
- integration tests (allow network & hardware access) - no autorun (if applicable)
- CI - unit tests for library (mock hardware & network) - autorun
- CI publishing (microbundle and push to npm)
- example site


### node server library

These are projects that are meant to run only on server-side.

<!-- put list here -->

They should have these setup:

- issue templates
- docs for API (either in README.md or API.md)
- update/audit all dependency packages regularly
- installation instructions
- es6 + microbundle
- FUNDING
- integration tests (allow network & hardware access) - no autorun (if applicable)
- CI - unit tests for library (mock hardware & network) - autorun
- CI publishing (microbundle and push to npm)


### node cli & library

These are projects that are a node library, and have a CLI that exposes most of the features 

- rawproto
- tplight

They should have these setup:

- issue templates
- docs for API (either in README.md or API.md)
- update/audit all dependency packages regularly
- installation instructions
- es6 + microbundle
- pkg on .cjs CLI entry-program & bin reference (for `npm i` or `npx`)
- self-help (tells user how to use it with `--help`)
- FUNDING
- integration tests (allow network & hardware access) - no autorun (if applicable)
- CI - unit tests for library (mock hardware & network) - autorun
- CI publishing (microbundle and push to npm)
- CI release - x86_64 (mac/win/linux) aarch64 (mac/linux) armv7l (linux)


### template project

These are projects that are meant to be extended to a user's project.

<!-- put list here -->

They should have these setup:

- issue templates
- usage instruction
- update/audit all dependency packages regularlys
- [github templates](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-template-repository)
- demo site (if applicable)
- FUNDING


### electron-style app

These are projects that are a desktop web-app

<!-- put list here -->

They should have these setup:

- issue templates
- installation instructions
- electron build (or eventually neutrolinojs, if possible)
- update/audit all dependency packages regularly
- FUNDING
- CI release - x86_64 (mac/win/linux) aarch64 (mac/linux) armv7l (linux)


### deployed site

Sometimes git is just used for pages. These projects should be clearly marked this way in README, and link back to the page they produce.

<!-- put list here -->


### docker

Since I want to link back to source for any published docker containers, there pporjects should have linkage both ways.

<!-- put list here -->

They should have these setup:

- issue templates
- usage instructions
- CI - docker build/publish
- FUNDING
- link to dockerhub in project "link" field
- link to github on dockerhub


### examples

Sometimes it's not really a template, but more of a an example of how to do something. These should be merged into a single project for all the related demos, like all the pakemon projects, as a way to show "here is 50 ways to make a graphical game intro"

<!-- put list here -->

They should have these setup for each sub-project:

- issue templates
- usage instructions
- update/audit all dependency packages regularly
- FUNDING


### other

Some projects don't fit into these categories. Just try to work out the best practices for that ecosystem (C++, python, PHP, etc) and follow them.

<!-- put list here -->

Some basic things these should have:

- issue templates
- usage instructions
- update/audit all dependency packages regularly
- FUNDING