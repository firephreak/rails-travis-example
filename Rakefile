#!/usr/bin/env rake
# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)

Triage::Application.load_tasks

Rake::Task[:default].clear

task :default => ["secure_pipeline:gauntlt"]

namespace :secure_pipeline do
  task :gauntlt do
    sh 'echo "JAMES"'
  end
end


