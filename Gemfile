source 'http://rubygems.org'
source 'https://gems.gemfury.com/vo6ZrmjBQu5szyywDszE/'

gem 'gds-warmup-controller'

# passenger compatability
group :passenger_compatibility do
  gem 'rack', '1.3.5'
  gem 'rake', '0.9.2'
end

group :router do
  gem 'router-client', '2.0.3', :require => 'router/client'
end

gem 'rails', '3.1.3'
gem 'rails-i18n'
gem 'json'
gem 'plek', '~> 0.1'
gem 'rummageable'
gem 'aws-ses', :require => 'aws/ses'
gem 'exception_notification'
if ENV['API_DEV']
  gem 'gds-api-adapters', :path => '../gds-api-adapters'
else
  gem 'gds-api-adapters', '~> 0.0.51'
end
gem 'htmlentities', '~> 4'

if ENV['SLIMMER_DEV']
  gem 'slimmer', :path => '../slimmer'
else
  gem 'slimmer', '~> 1.1.39'
end

if ENV['GOVSPEAK_DEV']
  gem 'govspeak', :path => '../govspeak'
else
  gem 'govspeak', '~> 0.8.15'
end

group :test do
  gem 'capybara', '~> 1.1.2'
  gem 'ci_reporter'
  gem 'factory_girl_rails'
  gem 'mocha', :require => false
  gem 'selenium-webdriver'
  gem "shoulda", "~> 2.11.3"
  gem 'webmock', :require => false
  gem "simplecov", "0.4.2"
  gem "poltergeist", "~> 0.6.0"
end

if ENV['RUBY_DEBUG']
  gem 'ruby-debug19'
end
