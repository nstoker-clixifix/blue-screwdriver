# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

gem 'coderay', '1.1.1'
gem 'rack-test', '0.7.0'
gem 'rspec', '3.6.0'
gem 'sequel', '4.48.0'
gem 'sinatra', '2.0.0'
gem 'sqlite3', '1.3.13'

group :development do
  gem 'guard'
  gem 'guard-brakeman'
  gem 'guard-bundler', require: false
  gem 'guard-rspec', require: false
  gem 'guard-rubocop'
  # gem 'guard-shotgun' # guard init shotgun needed also shotgun?
  gem 'rubocop', require: false
end
