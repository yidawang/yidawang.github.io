# Personal Website

## Development

### Prerequisites

- [Homebrew](https://brew.sh) (macOS)
- Ruby 3.2+ (install via Homebrew)
- Bundler

Install Ruby and Bundler:
```bash
brew install ruby
echo 'export PATH="/opt/homebrew/opt/ruby/bin:/opt/homebrew/lib/ruby/gems/4.0.0/bin:$PATH"' >> ~/.zprofile
source ~/.zprofile
gem install bundler
```

### Run locally
```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000 in your browser.

### Build
```bash
bundle exec jekyll build
```

### Notes
- The `Gemfile` uses `jekyll ~> 4.3` directly (instead of `github-pages`) for local preview, as `github-pages` pins to Jekyll 3.9 which is incompatible with Ruby 3.2+.
- GitHub Pages CI build is unaffected and deploys normally on push.
