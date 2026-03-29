source "https://rubygems.org"

ruby '3.4.7'

gem 'rails', '~> 8.0.0'
gem "pg", "~> 1.6"
gem "propshaft"
gem "puma", ">= 5.0"
gem "importmap-rails"
gem "turbo-rails"
gem "stimulus-rails"
gem "jbuilder"
gem 'mini_racer', platforms: :ruby
gem "redis", ">= 4.0.1"
gem "tzinfo-data", platforms: %i[ windows jruby ]
gem "bootsnap", require: false
gem "image_processing", "~> 1.13"

# Background + Auth
gem 'sidekiq'
gem "devise"

# Monitoring
gem 'sentry-ruby'
gem 'sentry-rails'
gem 'sentry-sidekiq'

# =========================
# 🛒 SPREE (LOCKED TO 5.3.5)
# =========================
spree_opts = '~> 5.3.5'

gem "spree", spree_opts
gem "spree_admin", spree_opts
gem "spree_storefront", spree_opts
gem "spree_emails", spree_opts
gem "spree_sample", spree_opts

# Extensions (SAFE)
gem "spree_i18n"

# ⚠️ IMPORTANT FIX (PIN VERSION)
gem "spree_stripe", "~> 1.5"

gem "spree_google_analytics", "~> 1.1"
gem "spree_klaviyo", "~> 1.1"

# =========================
# 🔌 CUSTOM GEMS (YOURS)
# =========================
gem 'spree_product_reviews', git: 'https://github.com/umeshravani/spree_product_reviews.git', branch: 'main'
gem 'spree_razorpay_checkout', git: 'https://github.com/umeshravani/spree_razorpay.git', branch: 'main'
gem 'spree_cod_payment', git: 'https://github.com/olympusone/spree_cod_payment.git', branch: 'main'
gem 'spree_google_products', git: 'https://github.com/umeshravani/spree_google_products', branch: 'main'

# =========================
# DEV / TEST
# =========================
group :development, :test do
  gem "debug", platforms: %i[ mri windows ]
  gem 'brakeman'
  gem 'dotenv-rails', '~> 3.1'
  gem 'rubocop', '~> 1.23'
  gem 'rubocop-performance'
  gem 'rubocop-rails'
  gem 'pry'
  gem 'pry-remote'

  # ✅ FIXED VERSION
  gem 'spree_dev_tools', '~> 0.5.0'
end

group :development do
  gem 'listen', '>= 3.0'
  gem "foreman"
  gem "web-console"
  gem "letter_opener"

  gem 'solargraph'
  gem 'solargraph-rails'
  gem 'ruby-lsp'
  gem 'ruby-lsp-rails'
end

group :test do
  gem 'rails-controller-testing'
end