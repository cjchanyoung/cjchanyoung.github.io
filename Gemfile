source "https://rubygems.org"

if RUBY_VERSION >= '3.2'
  Object.send(:define_method, :tainted?) { false }
  Object.send(:define_method, :taint) { self }
  Object.send(:define_method, :untaint) { self }
end

gem "jekyll", "~> 3.9.0"
gem "minimal-mistakes-jekyll"

group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-gist"
  gem "jekyll-paginate"
  gem "jekyll-sitemap"
  gem "jekyll-include-cache"
  gem "jekyll-algolia"
  gem "jemoji"
  gem "jekyll-remote-theme"
end

gem "csv"
gem "bigdecimal"
gem "webrick"
gem "base64"
gem "ostruct"
gem "logger"
gem "mutex_m"
gem "kramdown-parser-gfm"
gem "faraday-retry"

gem "wdm", ">= 0.2.0" if Gem.win_platform?