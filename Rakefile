desc 'outputs hello to the terminal'
namespace :greeting do 
  task :hello do 
    puts "hello from Rake!"
  end

  desc 'outputs hola to the terminal'
  task :hola do 
    puts "hola de Rake!"
  end
end

namespace :db do
  desc 'migrates changes to your database'
  task :migrate => :environment do 
    Student.create_table
  end

  desc 'seeds the database with sample data'
  task :seed do
    require_relative './db/seeds.rb' 
  end
end

desc 'start Pry console'
task :console do
  Pry.start
end


task :environment do
  require_relative './config/environment'
end