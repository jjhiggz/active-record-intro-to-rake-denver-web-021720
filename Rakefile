namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end
  desc 'outputs hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

task :environment do
   require_relative './environment.rb'
end

task :console => :environment do

end

namespace :db do
  task db:migrate => :environment do
    Student.create_table
  end
end
