# Copyright 2017 Google Inc.
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

source 'https://rubygems.org'

gem 'google-api-client'
gem 'googleauth'

group :test do
  gem 'fakeweb'
  gem 'puppet', ENV['PUPPET_GEM_VERSION'] || '~> 4.2.0'
  gem 'puppet-lint'
  gem 'puppet-lint-unquoted_string-check'
  gem 'puppet-syntax'
  gem 'puppetlabs_spec_helper'
  gem 'rake', '~> 10.0'
  gem 'rspec'
  gem 'rspec-mocks'
  gem 'rspec-puppet'
  # TODO(alexstephen): Monitor rubocop upsteam changes
  # https://github.com/bbatsov/rubocop/pull/4329
  # Change will allow rubocop to use --ignore-parent-exclusion flag
  # Current rubocop upstream will not check Chef files because of
  # AllCops/Exclude
  gem 'rubocop', git: 'https://github.com/nelsonjr/rubocop.git',
                 branch: 'feature/ignore-parent-exclude'
  gem 'simplecov'
end
