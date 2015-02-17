## Sensu-Plugins-librato

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-librato.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-librato)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-librato.svg)](http://badge.fury.io/rb/sensu-plugins-librato)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-librato/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-librato)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-librato/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-librato)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-librato.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-librato)

## Functionality

## Files
 *
 *
 *
 *

## Usage

**handler-metrics-librato**
```
{
  "librato": {
    "email": "email@example.com",
    "api_key": "12345",
    "use_sensu_client_hostname_as_source": false
  }
}
```

**handler-librato-occurrences**
```
{
  "librato": {
    "email": "email@example.com",
    "api_key": "12345"
  }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-librato -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-librato`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-librato' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-librato' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
