# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require File.expand_path('../config/application', __FILE__)

Rails.application.load_tasks

task :itest do
  sh %{[ -d verify ] && cd verify && sh setup.sh && npm install && npm run test}
end
