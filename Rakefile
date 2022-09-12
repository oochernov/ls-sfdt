# frozen_string_literal: true

require 'bundler/gem_tasks'
require 'rspec/core/rake_task'
require 'rake-version'
require 'rubocop/rake_task'

RuboCop::RakeTask.new
RSpec::Core::RakeTask.new(:spec)
Rake::Task['release'].clear

RakeVersion::Tasks.new do |v|
  v.copy 'lib/version.rb' # update single file
end

task default: %i[rubocop spec]
