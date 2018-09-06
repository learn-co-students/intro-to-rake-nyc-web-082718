

namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

desc 'outputs hello to the terminal'
  task :hola do
    desc "writes hola"
    puts "hola de Rake!"
  end
end

task :environment do
  require_relative './config/environment'
end


namespace :db do
  desc "creates access through environment"
  task :migrate => :environment do
    Student.create_table
  end

  desc "seeds database with data from seed file"
  task :seed do
    require_relative './db/seeds.rb'
  end
end
