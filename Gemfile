source "https://rubygems.org"

# Use the github-pages gem for full GitHub Pages compatibility
gem "github-pages", group: :jekyll_plugins

# Additional plugins
group :jekyll_plugins do
  gem "jekyll-feed"
end

# Windows and JRuby compatibility
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]
gem "webrick" # Required for Ruby 3.0+
