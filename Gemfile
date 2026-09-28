source "https://rubygems.org"

gem "jekyll", "~> 4.3.3"

# No longer bundled with Ruby 3.4+, which Jekyll 4.3 still requires.
gem "csv"
gem "base64"
gem "bigdecimal"
gem "logger"
gem "webrick", "~> 1.8"

platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end
gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]
