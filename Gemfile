source 'https://rubygems.org'

gemspec

gem 'mocha', '~> 0.14', require: false
gem 'rack-cache', '~> 1.2'
gem 'jquery-rails', '~> 3.1.0'
gem 'turbolinks'
gem 'coffee-rails', '~> 4.0.0'
gem 'arel', github: 'rails/arel', branch: 'master'
gem 'sprockets-rails', github: 'rails/sprockets-rails', branch: '2-1-stable'
gem 'bcrypt', '~> 3.1.7', require: false
gem 'uglifier', '>= 1.3.0', require: false
gem 'pony'

group :doc do
  gem 'sdoc', '~> 0.4.0'
  gem 'redcarpet', '~> 3.1.0', platforms: :ruby
  gem 'w3c_validators'
  gem 'kindlerb'
end

gem 'dalli', '>= 2.2.1'

local_gemfile = File.dirname(__FILE__) + "/.Gemfile"
instance_eval File.read local_gemfile if File.exist? local_gemfile

group :test do
  platforms :mri_19 do
    gem 'ruby-prof', '~> 0.11.2'
  end

  platforms :mri_19, :mri_20 do
    gem 'debugger'
  end

  gem 'benchmark-ips'
end

platforms :ruby do
  gem 'nokogiri', '>= 1.4.5'
  gem 'racc', '>=1.4.6', require: false
  gem 'pg', '>= 0.11.0'
end