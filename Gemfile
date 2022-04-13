# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION
DECIDIM_VERSION="0.25.2"

gem "decidim", DECIDIM_VERSION
gem "decidim-conferences", DECIDIM_VERSION
gem "decidim-consultations", DECIDIM_VERSION
# gem "decidim-elections", DECIDIM_VERSION
#gem "decidim-initiatives", DECIDIM_VERSION
gem "decidim-templates", DECIDIM_VERSION

# bug in version 1.9
gem "i18n", "~> 1.8.1"

gem "bootsnap", "~> 1.7"
gem "puma", ">= 5.0.0"
gem "faker", "~> 2.14"
gem "wicked_pdf", "~> 2.1"
gem "decidim-term_customizer", :ref => '12fbd0e', git: 'https://github.com/mainio/decidim-module-term_customizer'
gem "decidim-decidim_awesome"
gem "omniauth-rails_csrf_protection"

group :development, :test do
  gem "byebug", "~> 11.0", platform: :mri
  gem "decidim-dev", DECIDIM_VERSION
end

group :development do
  gem "letter_opener_web", "~> 1.4"
  gem "listen", "~> 3.1"
  gem "spring", "~> 2.0"
  gem "spring-watcher-listen", "~> 2.0"
  gem "web-console", "~> 4.0"

  gem "capistrano", "~> 3.14"
  gem "capistrano-bundler"
  gem "capistrano-passenger"
  gem "capistrano-rails"
  gem "capistrano-rails-console"
  gem "capistrano-rbenv"
  gem "capistrano-sidekiq"
end

group :production do
  gem "passenger"
  gem 'delayed_job_active_record'
  gem "daemons"
  gem "figaro"
end
