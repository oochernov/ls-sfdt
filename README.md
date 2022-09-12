# Template

TODO: Describe your gem
## Installation

This gem is pushed to an authenticated GitHub Packages.
Prior to installing this gem please follow the setup directions for [authenticating to github packages](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-rubygems-registry#authenticating-to-github-packages). If you have already complted this step for another private gem repository then it can be skipped.

Add this line to your application's Gemfile:

```ruby
gem 'template'
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install template
## Development

After checking out the repo, run `bundle install` to install dependencies. Then, run `rake spec` to run the tests.

To install this gem onto your local machine, run `bundle exec rake install`. 

# Versioning

This repository uses semantic versioning. 

By default, the main branch pipeline will increment patch versions.

To increment major or minor versions run the correct to `rake version` task prior to commit.
# Pipelines

## Main Branch Pipeline Flow
1. Install dependencies
1. Lint
1. Run tests
1. Increment patch version and create GitHub tag
1. Push new version to GitHub Packages store
## Pull Requests Piepline Flow
1. Install dependencies
1. Lint
1. Run tests

## Rake Tasks
``` 
rake build                 # Build template.gem into the pkg directory
rake build:checksum        # Generate SHA512 checksum 
rake clean                 # Remove any temporary products
rake clobber               # Remove any generated files
rake install               # Build and install template.gem into system gems
rake install:local         # Build and install template.gem into system gems without network access
rake rubocop               # Run RuboCop
rake rubocop:auto_correct  # Auto-correct RuboCop offenses
rake spec                  # Run RSpec code examples
rake version               # Show the current version
rake version:bump:major    # Bump the major version
rake version:bump:minor    # Bump the minor version
rake version:bump:patch    # Bump the patch version
rake version:set[value]    # Set the version (rake "version:set[1.2.3]")
```

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/LinkSquares/linksquares-template.
