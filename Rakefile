# frozen_string_literal: true

require 'bundler/gem_tasks'
require 'rspec/core/rake_task'
require 'rubocop/rake_task'

RSpec::Core::RakeTask.new(:spec)
RuboCop::RakeTask.new(:rubocop)

task default: %i[rubocop spec]

task :console do
  exec 'irb -r eventify_pro -I ./lib'
end

task :build do
  system 'gem build eventify_pro.gemspec'
end
