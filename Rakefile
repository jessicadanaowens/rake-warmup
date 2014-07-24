task :first do
  puts "First!"
end

task :second => :first do
  puts "Second!"
end

desc "Print a nice greeting"
task :greet do
  puts "What's your name"
  name = STDIN.gets.chomp
  puts "hello #{name}"
end

desc "Print the current time"
task :current_time do
  puts Time.new
end

desc "Prints the users favorite food"
task :print_favorite_food do
  puts "What is your favorite food"
  food = ENV["FAVORITE_FOOD"]
  puts "Your favorite food is #{food}"
end

namespace :morning_routine do
  task :wake_up do
    puts "wake up!"
  end

  task :get_dressed => :wake_up do
    puts "get dressed!"
  end

  task :eat_breakfast => :wake_up do
    puts "eat breakfast!"
  end

  task :brush_teeth => :eat_breakfast do
    puts "brush teeth"
  end

  task :ready_for_class => :brush_teeth do
    puts "get ready for class"
  end
end


namespace :greeting do
  desc "Say hello"
  task :hello do
    puts "Hello there"
  end

  desc "Say howdy"
  task :howdy do
    puts "Howdy partner"
  end
end