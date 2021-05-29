# open_geosciene_code_projects_viz

## Original Project Plan
https://github.com/softwareunderground/transform-2021-hackathon/discussions/14

The project plan has now been moved to issues: https://github.com/softwareunderground/open_geosciene_code_projects_viz/issues

## Slides on What's trying to be accomplished with this repository
https://observablehq.com/@justingosses/more-visible-connections-between-projects-can-nudge-devel 

## Live Pages
Explore page: https://softwareunderground.github.io/open_geosciene_code_projects_viz/explore/
Dependencies analysis: https://softwareunderground.github.io/open_geosciene_code_projects_viz/explore/dependencies/
Most popular repositories: https://softwareunderground.github.io/open_geosciene_code_projects_viz/explore/popular-repos/


## Types of Changes from LLNL Original
### LLNL content that is just removed or links to them take away
- Entire folders & markdown removed
  - About/index.md
  - About/FAQ
  - posts/*
  - news/*
  - radiuss/*
  - JS/Explore/pie_activityCommits.js
  - JS/Explore/pie_activityLines.js
  - JS/Explore/line_repoCreationHistory.js


### LLNL content that is swapped out
#### Swapped out individual words
- Most common = "LLNL" => "SWUNG"
- Less common = "LLNL" => ""
#### HTML Elements Removed
- Links to certain pages that have been replaced
  - header 
    - github repo
    - fork this repo
    - twitter
  - -in progress-
- Links to certain pages have been removed entirely:
    - header: -in progress-
    - homepage: -in progress-

### Configuration Changed in _config.yml
- replaced
```
url: "https://software.llnl.gov"
repo_u
```
with 
```
baseurl: "/open_geosciene_code_projects_viz"
```







------------

## Prerequisites

Before you begin, make sure you have working installs of Git, Ruby, and Bundler <https://bundler.io/> You will need these tools for development.

## Getting Started

To work locally, first clone into the repository:

```
git clone https://github.com/softwareunderground/open_geosciene_code_projects_viz.git
```

Make sure you are in the directory you just created by running `cd llnl.github.io` Then you can use `bundler` to install the Ruby dependencies (see the [Jekyll installation docs](https://jekyllrb.com/docs/installation/) for step-by-step guides to setting this up):

```
bundle install
```

Running this will install everything in your Gemfile (including Jekyll). Finally, run the development web server with:

```
bundle exec jekyll serve
```

Followed by opening <http://127.0.0.1:4000/open_geosciene_code_projects_viz/> in a web browser.


...............
...............
...............
...............
...............
...............
...............ORIGINAL FORKED REPO README BELOW...............
...............
...............
...............
...............
...............
# LLNL Software Catalog

Author: Ian Lee <lee1001@llnl.gov>

Welcome to the Lawrence Livermore National Laboratory software portal! The purpose of this software portal is to serve as a hub for open source software that is produced by Lawrence Livermore National Laboratory.

LLNL produces software on a daily basis. Some of this software is used only internally, other components are licensed for use by external partners and collaborators, still other software is released, or even actively developed, in the open on software hosting platforms such as GitHub.com, Bitbucket.org, Sourceforge.net, and others.

## Prerequisites

Before you begin, make sure you have working installs of Git, Ruby, and Bundler <https://bundler.io/> You will need these tools for development.

## Getting Started

To work locally, first clone into the repository:

```
git clone https://github.com/LLNL/llnl.github.io.git
```

Make sure you are in the directory you just created by running `cd llnl.github.io` Then you can use `bundler` to install the Ruby dependencies (see the [Jekyll installation docs](https://jekyllrb.com/docs/installation/) for step-by-step guides to setting this up):

```
bundle install
```

Running this will install everything in your Gemfile (including Jekyll). Finally, run the development web server with:

```
bundle exec jekyll serve
```

Followed by opening <http://127.0.0.1:4000/open_geosciene_code_projects_viz/> in a web browser.

### Tips

The gems in your sourcefile get updated frequently. It is a good idea to occasionally run `bundle update` from within your project's root directory to make sure the software on your computer is up to date.

Sometimes there can be dependency conflicts if your local version of Ruby is different from this repo or github pages deployment settings. You can find the version number of each of GitHub Page's current dependency's [here](https://pages.github.com/versions/). You can often avoid dependency issues if you use the same versions, including for Ruby. 

As an example, the default version of Ruby used to deploy GitHub Pages on github.com as of 2021-04-08 was Ruby	2.7.1. If you tried running Ruby version 3.0.0 locally on macOS, you'll need to do some extra steps to correctly install the dependencies for this repository. You'd need to run `bundle add webrick` as it is no longer a prepackaged dependency with Ruby in 3.0.0. You may also need to run `gem install eventmachine -- --with-openssl-dir=/usr/local/opt/openssl@1.1` as MacOS >10.14 doesn't use openssl from the same path as is still assumed to be in by eventmachine.

## Contact

If you have any questions or would like to request a private repository, please don't hesitate to contact [Ian Lee](mailto:ian@llnl.gov) or one of [the GitHub organization admins](mailto:github-admin@llnl.gov).

You can also find us on our mailing list: <open-source@llnl.gov>

# Release

The code of this site is released under the MIT License. For more details see the
[LICENSE](LICENSE) File.

LLNL-CODE-705597
LLNL-WEB-680594
