source 'https://rubygems.org'

gem 'rails', '6.1.7.3'

gem 'zip'
gem 'lograge', '>= 0.9.0'
# Allow using posix-spawn for popen to save memory with multiple threads.
gem 'posix-spawn'

#For Tasks/Search Providers
gem 'google-api-client', '~> 0.8.6'
gem "github_api", ">= 0.18.1", require: false
gem 'colorize', require: false
gem 'twitter', '>= 6.0.0'
gem 'market_bot'
gem 'koala'
gem "brakeman", ">= 3.3.0", require: false
gem "bundler-audit"
gem 'rest-client'
gem 'chartkick', '>= 3.4.0'
gem 'redcarpet', '>= 3.5.1'

gem 'addressable', '>= 2.8.0'

gem 'jwt', '<= 1.5.2'

# Pretty file sizes
gem 'filesize'

# scott things
gem 'json-schema-generator'
gem 'zeroclipboard-rails'

gem 'activerecord-session_store', git: 'https://github.com/rails/activerecord-session_store'
#Database gems
gem 'sqlite3'
gem 'pg'

#git functionality
gem 'git', '>= 1.13.0'

#Workflow
gem 'workflowable'

#JIRA Integration
#gem 'jiralicious'
gem 'jira-ruby'
#Authorization
gem 'cancan'

#Searching
gem 'ransack'

#Image processing/attachments
gem 'paperclip', '>= 5.2.1'
gem 'aws-sdk'
gem 'aws-sdk-ses'

# Time period parsing
gem 'chronic'

#Nice select fields
gem "select2-rails"

#Faster json parsing
gem 'oj'

#Bulk edits
gem 'activerecord-import'

#Used for task queueing
gem 'sidekiq', '>= 6.2.1'
gem 'sidekiq-status'
gem 'sidekiq-scheduler'
gem 'sidekiq-limit_fetch'
gem 'mlanett-redis-lock', require: 'redis-lock'

#Pagination
gem 'kaminari', '>= 1.2.1'

#Sidekiq UI
gem 'sinatra', '>= 2.2.3', require: false

#Templating language, not sure if used
gem 'slim'

#Performance gem that changes how links are handed
##gem 'turbolinks'
gem 'jquery-turbolinks'

#Allowing exporting/importing data into database
gem 'yaml_db', '>= 0.7.0'

#Authentication
gem 'devise', '>= 4.7.1'
gem 'responders', '>= 3.0.0'

#Comments
gem 'acts_as_commentable_with_threading'

#JSON API Calls
gem "active_model_serializers", ">= 0.10.12"

# Cron job generation
gem "whenever"

# Used for finding changes to serialized attributes
gem "hashdiff"

#gem 'active_scaffold'
gem "therubyracer"
gem "less-rails" #Sprockets (what Rails 3.1 uses for its asset pipeline) supports LESS
gem 'simple_form', '>= 5.0.0'

gem 'ip'

gem 'stackprof'

gem 'faraday'
gem 'net-http-persistent'

gem 'minitest'

gem 'minitest-rails', '>= 6.1.0'

group :development, :test, :production do
  gem 'unicorn'
  gem 'unicorn-rails'
end

group :test do
  #this doesn't get along with rack-mini-profiler
  gem 'oj_mimic_json'
end

# Used for Redis Cache
gem "redis-store", ">= 1.4.1"
gem "redis-rails"

group :development, :dirtylaundrydev do
  gem 'spring', group: :development
  gem "ruby-prof"
  gem 'meta_request', '>= 0.7.0'
  gem "binding_of_caller"
  gem "bullet"
  gem 'rack-mini-profiler', require: false
  gem 'flamegraph'
  gem 'rbtrace'
  #gem 'rails-footnotes'
  #gem 'rails-footnotes', github: 'josevalim/rails-footnotes', branch: 'release-4.0'
  gem 'rails-footnotes', '>= 4.0.2', '< 5'
  gem 'railroady'
  gem 'ruby_gntp'
  # gem 'rack-perftools_profiler', :require => 'rack/perftools_profiler'
end

group :development, :dirtylaundrydev, :profile do

  gem 'byebug'
  gem 'quiet_assets'
  gem "better_errors", ">= 2.8.0"
  gem 'pry'

end

#Testing
group :development, :test, :dirtylaundrydev do
  #gem 'rspec-rails'
  gem 'factory_girl_rails'

end

group :test do
  gem 'database_cleaner'
  gem 'shoulda', '~> 3.5', '>= 3.5.0'
  gem 'activerecord-nulldb-adapter'
  gem 'minitest-reporters'
  gem 'shoulda-matchers', '~> 2.6', '>= 2.6.2'
  gem 'shoulda-callback-matchers', '~> 1.1.4'
  gem 'simplecov', :require => false, :group => :test
end

gem 'foundation-rails', '5.3.3.0'
gem 'sass-rails', '6.0.0'
gem 'sass', '3.2.19'
gem 'coffee-rails', '4.2.2'
gem 'sprockets', '4.2.0'


gem 'uglifier', '>= 2.7.2'

gem 'jquery-rails', '>= 4.4.0'

gem 'rb-readline'

gem 'crack', '0.3.2'

# needed by  sidekiq
gem 'json', '>= 2.3.0'
gem 'ffi', '>= 1.9.24'


if File.exists?("custom/Gemfile")
  eval(IO.read("custom/Gemfile"), binding)
end
if File.exists?("../custom/Gemfile")
  eval(IO.read("../custom/Gemfile"), binding)
end
if File.exists?("./Gemfile.append")
  eval(IO.read("./Gemfile.append"), binding)
end
