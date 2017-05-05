
# frozen_string_literal: true
source "https://rubygems.org"

# gem "rails"

# Github-Pages (https://jekyllrb.com/docs/github-pages/)

source 'https://rubygems.org'

require 'json'
require 'open-uri'
versions = JSON.parse(open('https://pages.github.com/versions.json').read)

gem 'github-pages', versions['github-pages']
gem 'rmagick'
gem 'public_suffix', versions['2.0.5']
