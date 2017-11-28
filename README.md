> This repository is an unmaitained fork of the original country select in order to support 3-letter country codes. This can now be achieved using later versions of the country select gem, so you should probably use that instead.

# Rails – Country Select

Provides a simple helper to get an HTML select list of countries with
their [ISO 3166-1 alpha-3 codes](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3)
as values and [ISO 3166-1 names](https://en.wikipedia.org/wiki/ISO_3166-1)
as display strings. While it is a relatively neutral source of country
names, it may still offend some users.

Users are strongly advised to evaluate the suitability of this list
given their user base.

This has been adapted from https://github.com/stefanpenner/country_select

## Installation

Install as a gem using

```shell
gem install country_select
```
Or put the following in your Gemfile

```ruby
gem 'country_select', git: 'git://github.com/SplitIt/country_select.git'
```

## Tests

```shell
bundle
bundle exec rspec
```

## Example

Simple use supplying model and attribute as parameters:

```ruby
country_select("user", "country")
```

Supplying priority countries to be placed at the top of the list:

```ruby
country_select("user", "country", [ "gbr", "fra", "deu" ])
```

Copyright (c) 2008 Michael Koziarski, released under the MIT license
