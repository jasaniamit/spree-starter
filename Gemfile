# frozen_string_literal: true

source 'https://rubygems.org'
ruby '3.4.7'

# Spree Commerce (STABLE VERSION)
spree_version = '~> 5.3.5'

gem 'spree', spree_version
gem 'spree_admin', spree_version
gem 'spree_storefront', spree_version
gem 'spree_emails', spree_version

# Core Extensions
gem 'spree_i18n'
gem 'spree_stripe', github: 'spree/spree_stripe'
gem 'spree_google_analytics', '~> 1.1'

# Custom Features (your Git repos)
gem 'spree_product_reviews', git: 'https://github.com/umeshravani/spree_product_reviews.git', branch: 'main'
gem 'spree_razorpay_checkout', git: 'https://github.com/umeshravani/spree_razorpay.git', branch: 'main'
gem 'spree_cod_payment', git: 'https://github.com/olympusone/spree_cod_payment.git', branch: 'main'
gem 'spree_google_products', git: 'https://github.com/umeshravani/spree_google_products', branch: 'main'

# Rails & Infrastructure
gem 'rails', '~> 8.0.0'
gem 'pg', '~> 1.6'
gem 'puma', '>= 5.0'
gem 'redis'
gem 'sidekiq'
gem 'devise'

# Assets / UI
gem 'propshaft'
gem 'importmap-rails'
gem 'turbo-rails'
gem 'stimulus-rails'
gem 'tailwindcss-rails', '~> 3.3.1'

# Performance / Processing
gem 'bootsnap', require: false
gem 'image_processing', '~> 1.13'
gem 'aws-sdk-s3', require: false

# Logging / Monitoring
gem 'lograge'
gem 'sentry-ruby'
gem 'sentry-rails'
gem 'sentry-sidekiq'

# Search
gem 'meilisearch', '>= 0.28'

# Fix rubyzip future breaking change
gem 'rubyzip', '~> 2.3'

# Timezone
gem 'tzinfo-data', platforms: %i[windows jruby]

group :development, :test do
  gem 'debug', platforms: %i[mri windows]
  gem 'dotenv-rails'
  gem 'brakeman', require: false
  gem 'bundler-audit', require: false
  gem 'rubocop-rails-omakase', require: false
  gem 'simplecov-cobertura'
  gem 'spree_dev_tools', '>= 0.6.0.rc1'
end

group :development do
  gem 'web-console'
  gem 'listen'
  gem 'letter_opener'
end
