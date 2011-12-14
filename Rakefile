desc "Build the site"
task :build do
  sh "jekyll --no-auto"
end

desc "Deploy to heroku"
task :deploy => :build do
  sh "git push heroku master"
end
