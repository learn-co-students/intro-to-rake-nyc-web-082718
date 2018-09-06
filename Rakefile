task :environment do 
  require_relative './config/environment.rb'
end

desc 'drops to a Pry console'
task :console => :environment do
  Pry.start
end

namespace :greeting do 
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'prints hello in spanish'
  task :hola do 
    puts "hola de Rake!"
  end
end

namespace :db do 
  desc 'migrate changes to the database' 
  task :migrate => :environment do
    Student.create_table
  end

  desc 'populate db with dummy data' 
  task :seed do
    require_relative './db/seeds.rb'
  end
end
