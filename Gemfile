source "https://rubygems.org"

# Use Jekyll 4.x directly for local preview (github-pages pins to old versions
# incompatible with Ruby 3.2+; GitHub Pages itself still builds fine in CI)
gem "jekyll", "~> 4.3"

# Plugins (same as used on GitHub Pages)
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
end

# Windows and JRuby does not include zoneinfo files
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Performance-booster for watching directories on Windows
gem "wdm", "~> 0.1", platforms: [:mingw, :x64_mingw, :mswin]

# Lock `http_parser.rb` gem to `v0.6.x` on JRuby builds
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]
