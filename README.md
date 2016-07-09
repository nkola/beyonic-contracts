# Beyonic::Contracts
Uses [pacto](https://github.com/thoughtworks/pacto) to provide stubs against which you can write your own clients to the beyonic payment api.
It also provides integration contract testing against the beyonic api.

## Prerequisites
1. Install ruby if ruby is not installed already
2. `gem install bundler` if bundler is not installed already

## Usage

After checking out the repo, run `bin/setup` to install dependencies. and then run `bundle exec rake server:stub`
This will run a local server on port `9000` providing stubs for the beyonic payment api. You can change the port by running `bundle exec rake server:stub:8080`.

You can then make calls to the stub server as though you are working against the beyonic api it's self.

## Development
After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/nkola/beyonic-contracts.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
