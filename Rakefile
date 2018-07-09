


namespace :greeting do

  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outputs hola in espanol to the terminal'
  task :hola do
    puts "hola de Rake!"
  end

end


namespace :db do

  desc ' migrate changes to your db'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'sets up link to config/enviornment.rb'
  task :environment do
    require_relative './config/environment'
  end

  desc 'seed dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end

end
