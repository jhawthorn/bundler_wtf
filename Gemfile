source "https://rubygems.org"

branch = ENV.fetch('SOLIDUS_BRANCH', 'master')
gem "solidus", github: "solidusio/solidus", branch: branch
gem 'solidus_auth_devise'

if branch == 'master' || branch >= "v2.0"
  gem "rails-controller-testing", group: :test
end

gem 'pg'
gem 'mysql2'

group :development, :test do
  gem "pry-rails"
end

gemspec
