# Cacheflow

Colorized logging for Memcached and Redis

![Screenshot](https://gist.githubusercontent.com/ankane/64d630db934c5222587794232a690864/raw/880b70fdbd2d11ccc8475f4616397184918852e8/console.png)

Works with the Rails cache, as well as [Dalli](https://github.com/petergoldstein/dalli) and [Redis](https://github.com/redis/redis-rb) clients directly

## Installation

Add this line to your application’s Gemfile:

```ruby
gem 'cacheflow', group: :development
```

When your log level is set to `DEBUG` (Rails default in development), all commands to Memcached and Redis are logged.

## Features

To silence logging, use: [master]

```ruby
Cacheflow.silence do
  # code
end
```

To silence logging for only Sidekiq commands, use: [master]

```ruby
Cacheflow.silence_sidekiq!
```

## History

View the [changelog](https://github.com/ankane/cacheflow/blob/master/CHANGELOG.md)

## Contributing

Everyone is encouraged to help improve this project. Here are a few ways you can help:

- [Report bugs](https://github.com/ankane/cacheflow/issues)
- Fix bugs and [submit pull requests](https://github.com/ankane/cacheflow/pulls)
- Write, clarify, or fix documentation
- Suggest or add new features