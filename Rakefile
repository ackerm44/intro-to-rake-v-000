desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

namespace :db do
  desc 'migrate changes to database'
  task :migrate => :environment do 
    student.create_table
  end

  desc 'seed the databse with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end

  desc 'drop into Pry'
  task :console => :environment do
    Pry.start
  end
end