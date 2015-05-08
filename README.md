# Description

This cookbook provides support for installing the BrightBox builds of Ruby.

For more documentation on these builds, please see [the official brightbox documentation](http://blog.brightbox.co.uk/posts/next-generation-ruby-packages-for-ubuntu).

**Please Note:** If you're upgrading from an older version, the default action is to upgrade packages. To change this, you need to override `node['brightbox-ruby']['default_action']`.

# Requirements

## Platform:

* Ubuntu

## Cookbooks:

* apt

# Attributes

* `node['brightbox-ruby']['default_action']` - Default action for Ruby install. Available options: `:upgrade`, `:install`. Defaults to `:upgrade`.
* `node['brightbox-ruby']['version']` - The version of Ruby to install. Defaults to `"2.1"`.
* `node['brightbox-ruby']['install_dev_package']` - Install the dev package, which provides headers for gem native extensions. Available options: `true`, `false`. Defaults to `true`.
* `node['brightbox-ruby']['gems']` - Gems to be installed by default. Defaults to `["bundler", "rake", "rubygems-bundler"]`.
* `node['brightbox-ruby']['rubygems_version']` - The version of rubygems to enforce, or nil to use the default packaged version. Defaults to `nil`.

# Recipes

* brightbox-ruby::default - Adds the brightbox repository, installs the Ruby package, sets it as the default then installs a sane server gemrc and adds bundler, rake and rubygems-bundler gems to bootstrap your environment.

## Contributing

We encourage all community contributions. Keeping this in mind, please follow these general guidelines when contributing:

* Fork the project
* Create a topic branch for what you're working on (git checkout -b awesome_feature)
* Commit away, push that up (git push your\_remote awesome\_feature)
* Create a new GitHub Issue with the commit, asking for review. Alternatively, send a pull request with details of what you added.
* Once it's accepted, if you want access to the core repository feel free to ask! Otherwise, you can continue to hack away in your own fork.

Other than that, our guidelines very closely match the GemCutter guidelines [here](http://wiki.github.com/qrush/gemcutter/contribution-guidelines).

(Thanks to [GemCutter](http://wiki.github.com/qrush/gemcutter/) for the contribution guide)


# License and Maintainer

Maintainer:: Mojo Lingo LLC (<ops@mojolingo.com>)

License:: Apache 2.0
