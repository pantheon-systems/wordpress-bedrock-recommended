# Composer-enabled WordPress template

[![Unsupported](https://img.shields.io/badge/pantheon-unsupported-yellow?logo=pantheon&color=FFDC28&style=for-the-badge)](https://github.com/topics/unsupported?q=org%3Apantheon-systems)

This is Pantheon's recommended starting point for forking new [WordPress](https://wordpress.org) upstreams that work with the Platform's Integrated Composer build process. It ~is also~ is _intended to be_ the Platform's standard WordPress with Composer upstream.

Unlike with other Pantheon upstreams, the WordPress core install, which you are unlikely to adjust while building sites, is not in the main branch of the repository. Instead, it is referenced as dependencies within [Roots/Bedrock](https://roots.io/bedrock/) that are installed by [Composer](https://getcomposer.org).

## Unsupported software

_This tool is an early stage, proof-of-concept and is not recommended for use on production sites._

## TODOs

While the architecture and directory structure of this upstream is unlikely to change, some notable things need to happen before this upstream is fully ready for prime time.

* **Development script** - In the future, it would be beneficial to have a script that set up the `/packages/` folder for local development on those individual repositories, so that you could do all development within a single environment. This script would clone those repositories into `/packages/` so they would be used in place of the Packagist versions.

## Contributing

Contributions are welcome in the form of GitHub issues and pull requests. If you would like to propose a change, please fork [pantheon-systems/wordpress-bedrock-recommended](https://github.com/pantheon-systems/wordpress-bedrock-recommended) and submit a PR to that repository.

## Local development

The `/packages/` directory can be used as a local path repository if you want to do development on any of the `pantheon-systems` packages included in this project. Simply `git clone` any dependency package into `/packages/` and then `composer update` will use your local versions rather than the public ones managed by Packagist.