source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "3.1.2"

gem "rails", "~> 7.0.0"
gem "pg"
gem "puma"
gem "sass-rails"
gem "webpacker"
gem "turbolinks"
gem "jbuilder"
gem "bundle_outdated_formatter"
gem "bootsnap", require: false
gem "net-smtp"
gem "tailwindcss-rails", "~> 2.0"

group :development, :test do
  gem "byebug", platforms: [:mri, :mingw, :x64_mingw]
end

group :development do
  gem "web-console"
  gem "listen"
  gem "spring"
end

group :test do
  gem "capybara"
  gem "selenium-webdriver"
  gem "webdrivers"
end

gem "tzinfo-data", platforms: [:mingw, :mswin, :x64_mingw, :jruby]

group :development do
  gem "solargraph"
  gem "erb-formatter"
  gem "rufo"
end

group :development, :test do
  gem "debug"
  gem "rspec-rails"
  # gem "ruby-debug-ide"
  # gem "debase"
end
