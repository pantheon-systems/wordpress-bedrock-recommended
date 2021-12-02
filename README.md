# Composer-enabled WordPress template

This is Pantheon's recommended starting point for forking new [WordPress](https://wordpress.org) upstreams that work with the Platform's Integrated Composer build process. It ~is also~ is _intended to be_ the Platform's standard WordPress with Composer upstream.

Unlike with other Pantheon upstreams, the WordPress core install, which you are unlikely to adjust while building sites, is not in the main branch of the repository. Instead, it is referenced as dependencies within [Roots/Bedrock](https://roots.io/bedrock/) that are installed by [Composer](https://getcomposer.org).

## Contributing

Contributions are welcome in the form of GitHub issues and pull requests. If you would like to propose a change, please fork [pantheon-systems/wordpress-bedrock-recommended](https://github.com/pantheon-systems/wordpress-bedrock-recommended) and submit a PR to that repository.