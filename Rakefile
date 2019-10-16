# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require_relative 'config/application'
require 'rubocop/rake_task'

Rails.application.load_tasks

RuboCop::RakeTask.new

# This task can include anything that needs to be checked before the code
# is verified to be suitable for addition to the code base.
task :verify => [:rubocop, :spec]

