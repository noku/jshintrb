require "bundler/gem_tasks"
require "multi_json"
require "rspec/core/rake_task"

[:build, :install, :release].each do |task_name|
  Rake::Task[task_name].prerequisites << :spec
end

RSpec::Core::RakeTask.new

task :default => :spec
