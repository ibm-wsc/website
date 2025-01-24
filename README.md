# Standards for the IBM Z Ecosystem team 

This repository will be used to documentent standards as well as the environments for the IBM Z Ecosystem team.   The goal of this repository is to provide a single place for members to understand the standards for the systems, the processes to access the systems, the processes used for the systems.  This repository will link to others where appropriate.  

This repository will be published with gitpages to allow easy access and sharing and if appropriate can be added to w3 search to make it more findable.

If there are documenents that can not be visible to all of IBM we will create folders where markdown will still be used but those pages will not be published.  IF there is a need for tightly controled documenation, private repositories will be created.  


# Publishing Documentation Updates

This section describes the tools and steps need to update this repository's documentation.

## Getting Started

This repository uses `mkdocs` to generate a static website from GitHub flavored markdown.  `mkdocs` can be installed by following the installation directions provided on the `mkdocs` website (https://www.mkdocs.org/user-guide/installation/).

In addition to `mkdocs`, the published static site uses a theme called [material](https://github.com/squidfunk/mkdocs-material).  The theme can be installed using the following command:

```bash
pip install mkdocs-material
```

## Local Development

When creating or updating the content of the site, `mkdocs` can be used to serve the site locally.  The command below will build and serve the site from a local directory.

```bash
mkdocs serve
```

`mkdocs` will automatically rebuild the site as changes are made.

## Deploying Updates

When updates are ready for publication, the following command is used to generate the site and push the results to the `gh-pages` branch for hosting.

```bash
mkdocs gh-deploy
```