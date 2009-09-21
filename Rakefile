require 'rubygems'
gem 'hoe', '>= 2.3.0'
require 'hoe'

Hoe.plugin :git

Hoe.spec "loofah" do
  developer "Mike Dalessio", "mike.dalessio@gmail.com"
  developer "Bryan Helmkamp", "bryan@brynary.com"

  self.extra_rdoc_files = FileList["*.rdoc"]
  self.history_file     = "CHANGELOG.rdoc"
  self.readme_file      = "README.rdoc"

  extra_deps << ["nokogiri", ">= 1.3.3"]

  # note: .hoerc should have the following line to omit rails tests and tmp
  #   exclude: !ruby/regexp /\/tmp\/|\/rails_tests\/|CVS|TAGS|\.(svn|git|DS_Store)/
end

load File.join('rails_test', 'Rakefile')

