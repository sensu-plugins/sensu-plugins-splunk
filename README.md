## Sensu-Plugins-splunk

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-splunk.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-splunk)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-splunk.svg)](http://badge.fury.io/rb/sensu-plugins-splunk)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-splunk/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-splunk)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-splunk/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-splunk)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-splunk.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-splunk)

## Functionality

## Files
 * bin/handler-splunkstorm

## Usage

```
{
  "splunkstorm": {
    "project_id": "12345",
    "access_token": "abcde"
  }
}
```

## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-splunk -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-splunk`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-splunk' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-splunk' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
