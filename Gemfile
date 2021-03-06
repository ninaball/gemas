source "https://rubygems.org/"

ruby '2.2.1'
gem 'rails', '4.2.7.1'

gem 'active_presenter', '4.1.5'
gem 'activeresource', '4.1.0'
gem 'responders', '2.3.0'

# json template api
gem 'rabl', '0.14.1'
gem 'oj', '3.7.12'

# I18n database fields models
gem 'globalize', '5.0.1'
gem 'language_list', '1.0.0'
gem 'globalize-accessors', '0.1.5'
gem 'rails-i18n', '~> 4.0.3'

# Authentication
gem 'devise', '3.5.4'
gem 'devise_security_extension', '0.9.2'

# LDAP
gem 'net-ldap', '0.14.0'

# Security
gem 'rack-attack', '5.0.1'
gem 'secure_headers', '2.4.4'

# Authorization
gem 'six', '0.2.0'

# Misc
gem 'enumerize', '2.0.1' # AR enumerations
# Background jobs processing
gem 'sidekiq-unique-jobs', '5.0.10'
gem 'sinatra', '1.4.7', require: nil

gem 'configurations', '2.2.1' # Configurations

##gem 'stamp', '0.5.0' # Format dates

gem 'simple_form', '3.2.0' # Form helpers

gem 'pnotify-rails', '2.0.1.1'
gem 'unobtrusive_flash', '3.1.0'
gem 'bootstrap-switch-rails', '3.3.3'
gem 'font-awesome-rails', '4.7.0.1'
gem 'i18n-js', '2.1.2'
gem 'momentjs-rails', '>= 2.8.1'
gem 'bootstrap3-datetimepicker-rails', '~> 3.1.3'
gem 'bootstrap-datepicker-rails'

# gem 'introjs-rails', '1.0.0'

#  Views
gem 'hamlit-rails', '0.1.0'
gem 'hamlit', '2.6.1'

gem 'infinitescrolling-rails', '0.3.0'

gem 'pjax_rails', '0.4.0'
gem 'kaminari', '0.17.0'

gem 'factory_girl_rails', '4.5.0'

# Active Record Nesting
gem 'awesome_nested_set', '3.1.1'
gem 'the_sortable_tree', '2.5.0'

gem 'draper', '2.1.0'

gem 'rails-timeago', '~> 2.0'

# Connection pooling
gem 'connection_pool', '~> 2.2'

#group :assets do
# CSS related
gem 'sass-rails', '5.0.3'
gem 'compass-rails', '3.0.2'
gem 'bootstrap-sass', '3.3.7'

# Javascript related
gem 'coffee-rails', '4.2.1'

gem 'coffee-script-source', '~>1.10.0'

#TODO may be upgraded to 4.0.3
gem 'jquery-rails', '4.2.1' #jquery 1.10.2
gem 'jquery-cookie-rails', '1.3.1.1'

# fixed on top when scroll
gem 'scrollToFixed_rails', '1.0.5'

#icheck
gem 'icheck-rails', '1.0.2.2'

# Compression
gem 'uglifier', '3.0.3'

# Beesor documentation
gem 'beesor-docs', '~>4.1.0'
gem 'therubyracer', platforms: :ruby

gem 'sprockets', '2.12.4'

#client side template library
gem 'haml_coffee_assets', '1.16.2'
#end

group :test do
  gem 'cucumber', '2.0.0'
  gem 'capybara', '2.4.4'
  gem 'poltergeist', '1.7.0'
  gem 'capybara-screenshot', '1.0.4'
  gem 'capybara-slow_finder_errors', '0.1.2'
  gem 'database_cleaner', '1.5.3'

  gem 'cucumber-rails', '1.4.2.1', require: false

  # Next gem is commented because of the downgrade of cucumber to 1.3
  # due to parallel test and cucumber rerun problems

   # gem 'cucumber-rails', '1.4.2.1', :require => false

  # gem 'launchy', '2.4.3'
  # gem 'konacha', '3.3.0' # Javascript test with mocha framework
  gem 'simplecov', '0.12.0', require: false # Test coverage
  gem 'simplecov-rcov', '0.2.3', require: false # Test coverage
  gem 'shoulda-matchers', '2.7.0', require: false # AR validation testing
  gem 'enumerize-matchers', '0.0.2' # Enumerize validation
#  gem 'rubocop', '0.47.1' # Automatic Ruby code style checking tool

  # CI related
  gem 'ci_reporter', '2.0.0'
  gem 'ci_reporter_rspec', '1.0.0'
  #
  gem 'rails-dom-testing', '1.0.6'
end

group :development do
  # Preloading environment
  gem 'spring', '2.0.0'
  gem 'spring-commands-rspec', '1.0.4'
  gem 'spring-commands-cucumber', '1.0.1'
  gem 'rb-inotify', '0.9.7', require: false
  gem 'rb-fsevent', '0.9.8', require: false
  gem 'rb-fchange', '0.0.6', require: false
  gem 'libnotify' if /linux/ =~ RUBY_PLATFORM

  # Better error display
  gem 'better_errors', '2.1.1'
  gem 'binding_of_caller', '0.7.2', platforms: [:ruby]
  gem 'quiet_assets'

  # Code quality
  gem 'lol_dba', '2.1.1' #Db Index discovery

  # misc
  gem 'colored', '1.2' # Colored output to console
  gem 'annotate', '2.6.5'
  gem 'awesome_print'

  # Memory usage inspection
  gem 'derailed'
  gem 'stackprof'
  gem 'flamegraph'
  gem 'memory_profiler'
end

group :development, :staging do
  gem 'bullet', '5.4.2' #Detect N+1 query and eager loading
end

group :production, :staging do
  gem 'unicorn', '5.0.0', platforms: [:ruby]
  gem 'puma', '3.12.1', platforms: [:ruby], require: false
  gem 'thin', require: false
  #TODO la version 0.18.1 funciona en rails 4.2.1
  gem 'pg', '0.18.4', platforms: [:ruby]
  gem 'rb_cipher', '1.0.0'
end

group :test, :development do
  gem 'rspec-rails', '3.5.2'
  gem 'rspec-collection_matchers', '1.1.3'

  # RSpec matchers and Cucumber steps for testing JSON content
  gem 'json_spec', '1.1.4'

  # Javascript testing framework
  gem 'teaspoon-jasmine'

  # I18n verifications
  gem 'i18n-tasks', '0.9.5'
  #HACK TO AVOID ERROR ON I18N-TASK WITH SLOP 4.0 DEPENDENCY
  gem 'slop', '~> 4.4'
  gem 'axlsx', '2.0.1'
  gem 'axlsx_rails'

  # metrics dependencies
  gem 'brakeman', '3.1.5', require: false
  gem 'metric_fu', '4.12.0', require: false
  gem 'pronto', '0.4.1', require: false
  gem 'pronto-rubocop', require: false
  gem 'pronto-rails_best_practices', require: false
  gem 'pronto-flay', require: false
  #TODO poner y revisar compatibilidad
  gem 'pronto-brakeman', require: false
  gem 'pronto-haml', require: false
  gem 'pronto-reek', require: false
  #TODO poner y revisar compatibilidad
  gem 'pronto-scss', require: false
  #TODO poner y revisar compatibilidad
  # gem 'scss-lint', '0.30.0', require: false
  gem 'pronto-coffeelint', require: false
  gem 'faker', '1.6.6'
  gem 'parallel_tests', '2.10.0'
  gem 'coffeelint', '1.14.0'
end

gem 'dotenv-rails', '2.1.1' # Configuration
gem 'gon', '5.2.3'

gem 'render-q-mithril', '0.0.78'
gem 'amoeba', '3.0.0'
gem 'acts_as_list', '0.8.2'

gem 'public_activity', '1.4.2'
#date ranges validation
gem 'validates_overlap', '0.5.0'
gem 'rake', '10.4.2'

# Multi tenant
#TODO este se puede actualizar
gem 'apartment', '1.2.0' # active record multi-tenant
gem 'redis-namespace', '1.5.2' # redis multi-tenant

gem 'seedbank', '0.3.0'
gem 'redcarpet', '3.4.0' # Markdown

# License
gem 'lic_provider', '0.3.5'

# redis cache
gem 'redis', '3.3.5'
gem 'redis-store', '1.2.0'
gem 'redis-rails','5.0.2'
gem 'redis-activesupport','5.0.1'
gem 'redis-actionpack','5.0.2'
gem 'redis-rack', '2.0.5'
gem 'redis-rack-cache', '2.0.2'
gem 'rack-cache', '1.6.1'
# Better session storage support
gem 'redis-session-store', '0.9.2'

# JSON Api creator
gem 'grape', '0.11.0'

gem 'beesor_analytics', '1.0.4'
gem 'rack-mini-profiler', '0.10.1', groups: [:development, :staging], require: false
gem 'friendly_id', '5.1.0'
gem 'acts-as-taggable-on', '~> 4.0.0'
gem 'bootstrap_sortable_rails', '1.11.2'
gem 'activerecord-deprecated_finders'
gem 'rails_admin', '1.0.0'
gem 'rails_admin_globalize_field', '0.4.0'

# Log publishing
gem 'logstasher', '1.2.1'
# gem 'logstash-logger', '0.8.0'
# gem 'lograge', '0.3.1'
# gem 'logstash-event', '1.2.02'

gem 'mongoid-grid_fs'
gem 'moped', '2.0.7'
gem 'rubyzip'
gem 'yaml_db', '0.4.0'

gem 'pluck_to_hash'
# Version 3.1.2 is available but can not upload a zip to gridfs with this
gem 'bson', '3.2.6'

gem 'simple_captcha2', require: 'simple_captcha'

gem 'sequenced', '3.1.1'

gem 'puma_worker_killer', '0.1.1'

gem 'tzinfo-data', '1.2016.10'

gem 'exception_notification', '4.2.2'
