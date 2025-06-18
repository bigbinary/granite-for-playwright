# frozen_string_literal: true

source "https://rubygems.org"

ruby "3.2.4"

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails', branch: 'main'
gem "rails", "7.0.5"

# Use sqlite3 as the database for Active Record in dev and test envs
gem "sqlite3", "~> 1.4", group: [:development, :test]

# Use postgres in production since Heroku doesn't support SQLite
gem "pg", group: [:production]

# Use Puma as the app server
gem "puma", "~> 4.1"

# Use SCSS for stylesheets
gem "sass-rails", ">= 6"

# Transpile app-like JavaScript. Read more: https://github.com/shakacode/shakapacker
gem "shakapacker"

# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem "jbuilder", "~> 2.7"

# Use Active Model has_secure_password
gem "bcrypt", "~> 3.1.13"

# Reduces boot times through caching; required in config/boot.rb
gem "bootsnap", ">= 1.4.2", require: false

# For periodic jobs on sidekiq
gem "sidekiq-cron"

# For handling authorization
gem "pundit"

# React
gem "react-rails"

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem "tzinfo-data", platforms: %i[mingw mswin x64_mingw jruby]

# For patch level verification
gem "bundler-audit"

# For background jobs
gem "sidekiq", "<7"

group :development do
  # Preview email in browser
  gem "letter_opener"

  # Reenable after https://github.com/rails/rails/issues/26158 is fixed
  gem "listen", "~> 3.2"

  # Access an interactive console on exception pages or by calling 'console' anywhere in the code.
  gem "web-console", ">= 3.3.0"

  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem "spring", ">= 3"
  gem "spring-watcher-listen"

  # For code formatting and linting
  gem "rubocop", require: false
  gem "rubocop-rails", require: false
  # For linting ERB files
  gem "erb_lint", require: false, git: "https://github.com/Shopify/erb-lint.git", branch: "main"
end

group :test do
  # For generating test coverage report
  gem "simplecov", require: false
end

group :development, :test do
  # Rails integration for factory_bot, a replacement for fixtures
  gem "factory_bot_rails"

  # For auto-generating demo data
  gem "faker"

  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem "byebug", platforms: %i[mri mingw x64_mingw]

  # To load the environment variables
  gem "dotenv-rails"
end

gem "database_cleaner"

# PDF generation gem
gem "wicked_pdf"

# wicked_pdf uses the following binary
gem "wkhtmltopdf-binary"

# Required by ActiveStorage to use the GCS
gem "google-cloud-storage"
