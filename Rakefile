# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)
require 'rake'

Catarse::Application.load_tasks

if Rails.env == 'production'
    Rake::Task["db:structure:dump"].clear
end
