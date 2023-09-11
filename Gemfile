source :gemcutter
source "http://gems.github.com/"

gem "gas2", "0.1.8"
gem "cfoundry", "4.6.2"
gem "rubyzip", "0.9.9"

platforms :ruby_18 do
  gem "SystemTimer"
end

platforms :ruby_18 do
  gem "fastercsv"
end

group :development do
  platforms :ruby_18 do
    gem "ruby-debug"
    gem "metric_fu"
  end

  # Only one of these is required, but for dependency resolution
  # to work correctly, both have to be specified
  gem "thin"
  gem "unicorn"

  gem "sprockets"
  gem "capistrano"
end

group :production, :stw_production, :stw_staging, :staging, :atex_production, :wd_production, :cossette_production do
  gem "thin"
end


# vim: filetype=ruby
