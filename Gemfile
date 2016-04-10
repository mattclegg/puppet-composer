#ruby=1.9.3@puppet-composer

if ENV.key?('PUPPET_VERSION')
  puppetversion = "= #{ENV['PUPPET_VERSION']}"
else
  puppetversion = ['>= 2.7']
end

source 'https://rubygems.org'

gem 'puppet', puppetversion
gem 'puppetlabs_spec_helper'
gem 'rake', '< 11'
gem 'rspec-puppet', :git => 'https://github.com/rodjek/rspec-puppet.git'
gem 'rspec', '< 3.0.0'
gem 'mocha'
gem 'puppet-lint'
gem 'hiera'
gem 'hiera-puppet'

group :acceptance do
  gem 'beaker',                        :require => false
  gem 'beaker-rspec',                  :require => false
  gem 'beaker-puppet_install_helper',  :require => false
end
