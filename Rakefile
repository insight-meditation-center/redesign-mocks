require 'colorize'

task :build do
  puts 'Ensuring imc-bootstrap-sass submodule has dependencies installed...'.blue.bold
  exec_command('cd imc-bootstrap-sass && bundle install')

  puts 'Compiling CSS to css/...'.blue.bold
  exec_command('cd imc-bootstrap-sass && rake compile[../css]')

  puts 'Copying JS to js/...'.blue.bold
  exec_command('mkdir js && cp imc-bootstrap-sass/assets/javascripts/bootstrap.min.js js/')
end

def exec_command(cmd)
  puts "  #{cmd}".green
  puts `#{cmd}`.split("\n").map {|l| "  #{l}"}.join("\n")
end
