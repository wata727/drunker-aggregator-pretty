# Drunker::Aggregator::Pretty

**[DEPRECATED] This aggregator was integrated into Drunker.**

Default aggregator for [Drunker](https://github.com/wata727/drunker).

## Installation

    $ gem install drunker-aggregator-pretty

## Output Format

Display build ID and STDOUT, STDERR, exit status for each build.

```
-------------------------------------------------------------------------------------------
BUILD_ID: drunker-executor-1494140968:59c0b89f-099e-482c-8995-659f8b6b8523
RESULT: SUCCESS
STDOUT: ................

Finished in 0.12019 seconds (files took 0.14562 seconds to load)
16 examples, 0 failures

STDERR:
EXIT_STATUS: 0
-------------------------------------------------------------------------------------------


-------------------------------------------------------------------------------------------
BUILD_ID: drunker-executor-1494140968:f6cb0396-3005-44ca-8221-33b29cbbd309
RESULT: SUCCESS
STDOUT: ..........................................................................

Finished in 0.15774 seconds (files took 0.19026 seconds to load)
74 examples, 0 failures

STDERR:
EXIT_STATUS: 0
-------------------------------------------------------------------------------------------


-------------------------------------------------------------------------------------------
BUILD_ID: drunker-executor-1494140968:620c471e-19e7-48da-95e7-42cd66728455
RESULT: SUCCESS
STDOUT: ...........................................

Finished in 5.56 seconds (files took 0.14991 seconds to load)
43 examples, 0 failures

STDERR:
EXIT_STATUS: 0
-------------------------------------------------------------------------------------------
```

## Exit Status

Returns the maximum value of the exit status of each build. If the build failed, it will be treated as returning exit status 1.

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/wata727/drunker-aggregator-pretty. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

