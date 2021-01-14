# Rubocop::Inspire

This is the Inspire Ruby Style Guide

## Usage

Add this line to your application's Gemfile:

```ruby
gem 'rubocop-inspire', require: false
```

Add this to your project `.rubocop.yml` file

```ruby
inherit_gem:
  rubocop-inspire: rubocop.yml
```

And then execute:

    $ bundle install

You can continue to add application-specific rules/overrides in the
`.rubocop.yml` file in the root of your application, including annotating
your todo list:

```ruby
inherit_from: .rubocop_todo.yml
```

## Development

### Testing locally

In your application, use the `path` attribute to point to your local copy of the gem

```ruby
    # Use the relative path from your application, to the rubocop-inspire folder
    gem 'rubocop-inspire', path: '../rubocop-inspire', require: false
```

### Publishing the gem

If you have access to publish the gem on rubygems:

1. Update the `version.rb` file as appropriate
1. `bundle` if any dependencies  have changed
1. Commit all changes
1. Update the `CHANGELOG.md`
1. Publish to rubygems:
  1. `rake build`
  1. `cd pkg`
  1. `gem push rubocop-inspire.<version_number>.gem`


## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/DWPHoldings/rubocop-inspire.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
